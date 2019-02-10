##Intro
This a checklist that can be used for a typical marketing HTML/CSS site

##Setup
**Content**<br>
*Obtain all site content and assets* 
1. Site design
   - Or Zelpin link
1. Images/icons
   - Or insure that all assets are in Zeplin and exportable 
1. Menu design and behavior if any
  
**Credentials / Info Needed**
- Domain Registrar
- Form notification to email address
- Form notification from address
- URL of site
- Form confirmation from email address
- Form confirmation to email address
- Form confirmation reply-to email address
- Google maps API key
  - Or create key using dev account
- Instagram Feed
  - Obtain Credentials
  - Login with account that will be used to pull the feed from
  - Generate Access Token http://instagram.pixelunion.net/ 
  - Create API Client
  - Login with dev account that is used to manage API clients
  - https://www.instagram.com/developer/clients/manage/
  - To resolve recaptach issue enable “Disable Content-Security-Policy” extension
  
**Task list**
- Create task for developer  

##Checklist
**Styling**
- Favicon has been added and looks right
- Mobile styles all look right
- All colors used match the branding
- Smooth scroll

**Forms**
- Email is submitting
- Validation is working on required fields
- Confirmation message looks right
- Email is not going to spam
- Email subject is correct

**Information**
- Links are all working and going to correct account
- Phone numbers and addresses are all correct
- Google map is at the correct location
- Map pin is at correct location

**Go live**
- Hosting
- Add site to hosting account
- Upload files (or setup GIT and CD pipeline)
  - Whilst IP address for developer if needed 
- Update DNS
  - Add site to Cloudflare
  - Update name servers
  - Add A record and CNAME for www
- Setup SSL
  - Setup LetsEncrypt 
- Update htaccess to force SSL (or enforce via Cloudflare)
