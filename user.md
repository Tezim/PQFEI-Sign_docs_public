# User and UI Documentation

## Table of Contents

1. [Getting Started](#getting-started)

    1.1 [Installation](#installation)

    1.2 [Application startup](#application-startup)

    1.3 [User Registration](#user-registration)

2. [Authentication](#authentication)

    2.1 [Email-Password Login](#email-password-login)

    2.2 [Google Sign-In](#google-sign-in)
3. [Application](#application)
    
    3.1 [User profile](#user-profile)

    3.2 [Homepage](#homepage)


## Theme

---

<div align="center">
    <img src = "img/primary.png" alt="primary" width="96"> 
    <img src = "img/secondary.png" alt="Secondary" width="96">
    <img src = "img/tertiary.png" alt="Tertiary" width="96">
    <img src = "img/netral.png" alt="Neutral" width="96">
</div>

<div align="center">

<span style="color:#0039A6; padding: 20px">
#0039A6
</span>
<span style="color:#3858B7; padding: 20px">
#3858B7
</span>
<span style="color:#aa86a4; padding: 20px">
#aa86a4
</span>
<span style="color:#919094; padding: 20px">
#919094
</span>

</div>

## Getting Started

### Installation

### Application startup
After opening application, internet connection will be checked. If the internet connection is unavailable
user cannot enter the application and will be asked to check connection again.

<div align="center">
    <img src="img/UI/launcher_check.jpg" height="400">
    <img src="img/UI/launcher_check_fail.jpg" height="400">
</div>

### User Registration

1. Launch the app.
2. On the welcome screen, select "Sign up"
3. Enter your email and create a secure password.
4. Follow the prompts to complete the registration.


Any of following error messages can be displayed:
- invalid email
- Min. 6 and max. 12 characters
- Invalid password
- Passwords do not match

**Google Sign in**
1. Launch the app.
2. On the welcome screen, select "Sign up"
3. Click on Google logo
4. Follow the prompts to complete the registration.

Upon Failed registration all input fields will be emptied. Upper left corner contains back arrow to return to
main page.

<div align="center">
    <img src="img/UI/register.jpg" height="400">
    <img src="img/UI/registration-error-message.jpg" height="400">
</div>

## Authentication

<div align="center">
   <img src="img/UI/main-sign-in.jpg" height="400">
</div>

### Email-Password Login

1. Open the app.
2. Enter your registered email and password.
3. Tap "Sign in"

### Google Sign-In

1. Open the app.
2. Select Google image on the screen.
3. Choose your Google account to authenticate.

### Password reset

1. Open the app.
2. Select "Forgot password".
3. Fill in your email.
4. Tap "Send"
5. Follow instructions from received email to finish password reset

<div align="center">
   <img src="img/UI/pwd-reset.jpg" alt="email-reset" height="400">
</div>

<div align="center">
   <img src="img/reset-email.png" alt="email-reset">
</div>

### Log in / Log out splash screen

---

## Application

### User Profile
Profile settings management, key management excluded. The app provides simple and straightforward card design for better
UX. Danger zone provides "dangerous" user actions such as deleting and resetting account -> this part is red highlighted.

Main card shows lock icon (possible change to user profile picture), user handle-unique user ID, email of current
user and visible Sign Out button. Main card has scrollview to be more comfortable for user on different devices.

<div align="center">
    <img src="img/UI/profile_page.jpg" height="400">
</div>


**Account** 
- Share User Handle 
   
   - Creates QR code of user ID and shows it to user via Bottom sheet dialog
   - Navigation - swipe down or touch screen to close dialog

<div align="center">
    <img src="img/UI/user_handle.jpg" height="200">
</div>

- Reset Password

   - Send reset email to currently signed user (not possible for google sign in accounts)
   - Shows to user message based on the outcome - "email sent", "failed to send email"

**Support**
- Documentation

   - Redirects user to specified website - this public documentation
- Contacts

   - Redirects user to contacts page - currently contacts file in this repository
  
**Danger zone**

<div align="center">
    <img src="img/UI/danger-zone.jpg" height="200">
</div>

- Reset Account (Beta) currently disabled

   - Resets account - deletes all documents and keys of currently signed in user
   - Warning dialog is displayed to ask user for confirmation of this action

- Delete Account
   
   - Deletes all user information from database and account
   - Warning dialog is displayed to ask user for confirmation of this action

<div align="center">
    <img src="img/UI/confirm-dialog.jpg" height="400">
</div>

### Homepage 

After sign in homepage appears for user to choose what action to continue with.

### Key management
 
### Documents Management

**To be continued...**
