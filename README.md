# QA-LoginPageTestCase
The test case is to check that whether inputted email address and password are valid or not for Project QA-LoginPage. According to requirements, the lengths of email address and password are 2 to 20 characters and 6 to 40 characters, respectively.

### Test Case 1 - Verify the user can login successfully with email address and password. 

Example Data: 
- Email address: sam@gmail.com
- Password: 123456

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Login successfully to dashboard page and a pop up message to show that "Welcome!"

### Test Case 2 - Verify the user cannot login if email address and password do not match.

Example Data: 
- Email address: sam@gmail.com
- Password: 888888

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Cannot login successfully to dashboard page and a pop up message to show that "Invalid email address or password"

### Test Case 3 - Verify the user cannot login if email address or password is empty.

Example Data: 
- Email address: ' '
- Password: 123456

- Email address: sam@gmail.com
- Password: ' '

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Cannot login successfully to dashboard page and a pop up message to show that "Email address and password cannot be empty."

### Test Case 4 - Verify the user cannot login if email address out of range.

Example Data: 
- Email address: s@gmail.com
- Password: 123456

- Email address: sammmmmmmmmmmmmmmmmmmm@gmail.com
- Password: 123456

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Cannot login successfully to dashboard page and a pop up message to show that "The length of email address should be between 2 and 20 characters."

### Test Case 5 - Verify the user cannot login if password out of range.

Example Data: 
- Email address: sam@gmail.com
- Password: 12345

- Email address: sam@gmail.com
- Password: 123456123456123456123456123456123456123456123456

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Cannot login successfully to dashboard page and a pop up message to show that "The length of password should be between 6 and 40 characters."

### Test Case 6 - Verify email address is case-insensitive.

Example Data: 
- Email address: sam@gmail.com
- Password: 123456

- Email address: SAM@GMAIL.COM
- Password: 123456

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Login successfully to dashboard page and a pop up message to show that "Welcome!"

### Test Case 7 - Verify the the user cannot login if email address contains special character(s).

Example Data: 
- Email address: sa'm@gmail.com
- Password: 123456

- Email address: s!am@gmail.com
- Password: 123456

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Cannot login successfully to dashboard page and a pop up message to show that "Sorry, no secial character in email address."


### Test Case 8 - Verify the user cannot login if the format of email address does not follow "aa@bbb.ccc". 

Example Data: 
- Email address: sam@gmailcom
- Password: 123456

- Email address: samgmail.com
- Password: 123456

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Cannot login successfully to dashboard page and a pop up message to show that "Sorry, invalid email format."

### Test Case 9 - Verify the user cannot login if the email address does not start with a letter.

Example Data: 
- Email address: 8sam@gmailcom
- Password: 123456

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- Cannot login successfully to dashboard page and a pop up message to show that "Sorry, invalid email format."

### Test Case 10 - Verify password display "*********".

Example Data: 
- Email address: sam@gmail.com
- Password: 123456

Steps: 
- Input email address 
- Input password
- Click “Sign up” button

Expect result:
- The password will be displayed by asterisk (*/) when user is entering

### Test Case 11 - Verify the user cannot access the resource protected by login page directly.

Example Data: 
- URL of dashpage

Steps: 
- click URL of dashpage

Expect result:
- Login page will be display and ask user to re-login
