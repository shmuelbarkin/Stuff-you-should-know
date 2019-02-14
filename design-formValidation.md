# Form validation 
## Introduction 
When a user fills in a form on a webpage there are quite a few things that need to be addressed to provide the best user experience. One of those items are form validation, below are some pointers.
## Pointers
- Avoid errors in the first place
	- Use field input mask where applicable (make it impossible to put in an incorrectly formatted date in a date field)
	- Use clear labels, placeholder text and add explanatory text or tooltips as needed
- Show errors as soon as possible 
  - Check errors as soon the user leaves the field (if the error can be determined based on that cells input)
  - If the error can only be determined based on the contents of more than one cell, then check for the error as soon as the user has entered data into all relevant cells
  - Some errors will need to wait until form submit (e.g. a credit card is being processed)
- Don't show the error too early 
  - Don't show validation error until the user has left the field check for validation
  - At the same time - do remove validation as soon the issue has been fixed (before the user leaves the cell
- Provide positive feedback if applicable 
	- If they got it right - give 'em a check!
- Clear error messages
	- Don't make the user figure out that there is an issue or what the issue is
	- Make it clear that there is an error, users will often overlook a small print or a bit of red
	- Provided detailed error messages, so its clear to the user what needs to be fixed
	- If there is an error and the user hits submit the page should scroll up the first error (this is especially important when the error is out of view such as a long form or on mobile)
- reCAPTCHA
	- Use [Invisible reCAPTCHA](https://developers.google.com/recaptcha/docs/invisible)
	- You would be surprised how many users don't realize they need to click that box!
- Monitor 
	- Like with all UX - use [fullstory](https://www.fullstory.com) to see how your users interact with the form and where they are getting stuck.