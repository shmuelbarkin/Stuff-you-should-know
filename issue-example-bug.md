**Steps to reproduce**

1. Navigate to https://zurfly.com
2. Hover over "sellers" from the absolute top navigation
3. Click on "register as seller"
4. Fill in "first name", "last name", "email address", "password" and "confirm password"
5. Click on "Sign up now"

**Expected result**

1. The user gets an on screen notification that he is registered as a seller.
2. The user gets an email with his registration information.
3. The admin gets an email notifying them that a new seller registered.
4. The seller account is registered, and we can see it in the admin by navigating to Marketplace=>Manage Sellers

**Actual Result**

1. The user gets an error message 
	Fatal error: Call to a member function `getCountry()` on a non-object in `/chroot/home/zurflyco/zurfly.com/html/app/code/local/Apptha/Marketplace/Helper/Order.php on line 142`
2. The user doesn't get an email with his registration information.
3. The admin doesn't an email notifying them that a new seller registered.
4. The seller account is registered, and we can see it in the admin by navigating to Marketplace=>Manage Sellers

**Error Environment**
1. Users: any
2. Browser: Chrome Windows 
3. OS: Windows 10
4. URL of issue: https://zurfly.com/signup.html

**Additional Information**

1. I don't know for a fact that the user is meant to get an email - I'm just assuming he's supposed to
2. I don't know that the admin is supposed to get an email - I'm just assuming he's supposed to.
3. If they're meant to get an email, it is likely further on in the registration process but since it dies on the fatal error it never sends emails.