# Form validation

## Introduction
When a user fills in a form on a web page there are quite a few things that need to be addressed to provide the best user experience. One of those items is form validation, below are some pointers.

## Pointers
- Avoid errors in the first place
	- Use field input mask where applicable (make it impossible to put in an incorrectly formatted date in a date field)
	- Use clear labels, placeholder text and add explanatory text or tooltips as needed
	- Remove leading and trailing spaces on fields that a space will trigger a validation error (email address, zip code…)
- Show errors as soon as possible 
  - Check errors as soon the user leaves the field `onblur` (if the error can be determined based on that cells input)
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
	
## Internalization
*Internalization, when creating a form that is taking input from users in multiple countries some fields need to factor in the varying conventions used*
- Phone numbers
	- Insure you input mask works for all countries
	- If most of your users are from the US you can use a input mask that will format the numbers based on this xxx-xxx-xxxx but if the user has more or less than 10 digits the mask is removed
	- If there are more than 10 digits the mask is removed as the user types, if there are less than 10 digits the mask is removed `onblur`
- Address
	- State - this is typically only used in the US, if the user chooses Canada the label and options should change to `Province`, if any other country is chosen, this field should be hidden 
	- Zip code - only in the US is this called a `Zip code`, if any other country other that US is chosen the label should change to `Postal code`
	- Zip code validation - if you use Zip code validation make sure the validation is based on country. If you don't have a **reliable** validation regex for a specific county it's better to skip validation entirely (typically I skip validation for any county other US or Canada)
