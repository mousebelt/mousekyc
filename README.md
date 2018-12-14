# mousekyc
## An open source, image file uploading and user registration system

### Description
This project is created by MouseBelt and No Rest Labs to serve as an open-source and easily customizable solution that helps with KYC. Many regulations that bind financial companies in a KYC ("Know Your Customer" / "Know Your Client") process also apply to crytocurrency projects. We have a simple utility that can be plugged into an ICO dashboard, exchange or other cryptocurrency wallet subject to those regulations that will help collect the necessary user info for compliance.

### What does it do?
It's a user registration and login system which allows uploading of face images using the webcam api. There is an admin interface side which can control the submissions. The codebase is in javascript, react and node.js. It uses MongoDB for the database and can be installed quickly using [Docker](https://docker.com/).


### Do I Want This?

While it is an open source project and great learning experience, you should consult a legal advisor for production use, which we are not a substitute for. Typically, a KYC feature is required for ICO's and exchanges.

### Project Structure

Consists of three components:
* User registration web interface
* Backend server application
* Admin interface


**You will need to clone these 3 repos individually and follow the instructions within each one.**

1. **User registration web interface - **
(https://github.com/norestlabs/mousekyc-fe)   This is a react application that serves as the frontend for user registration. Registration is initiated by a user email and an authentication key sent from the backend of whichever service is connected, then a token to begin registration is returned. A user is then redirected and may upload an identity document, selfie with the identity document, and fill out fields with any required information for an admin to review.

2. **Backend server application - **
(https://github.com/norestlabs/mousekyc-be)   This is the backend, based in nodejs and mongodb. It serves both the admin and end user APIs. It can be customized to fit your application needs, and with a webhook going to the application you are trying to KYC. You can integrate an email provider by registering an account, making the appropriate DNS entries, and pasting in the keys to the application if you would like to send email notifications through this component as well.

3. **Admin interface - **
(https://github.com/norestlabs/mousekyc-admin)  This is the admin panel. It should be configured to aim at the backend, and with an application owner email specified in the configuration.

### Documentation

[**API Docs**](https://github.com/norestlabs/mousekyc-be/wiki) - You can view the API documentation in the wiki. Click through the bar on the right to page through the different APIs.

### Contributing

If you see a change, bugfix or other edit to make, please file an issue and open a PR. We'll be happy to review it and get it merged in.

### Usage

Use the repository however you like under the MIT license. Feel free to copy it and brand it to your product (instructions for this may be found in the frontend repository)
