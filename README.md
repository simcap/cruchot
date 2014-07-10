Cruchot is a service that handles email verification & confirmation
on your behalf for users who sign up to your service.

As a startup, it means you can build web applicaitons with full user registration
without the need to implement the email confirmation yourself.

Also you do not have to subscribe yourself to a email sender 
service to handle the signup.

You can choose different level of email checks

## Install

    gem install 'cruchot'

## Usage

    ....
    user_email = 'ludovic@gmail.com'

    Cruchot.verify(user_email)
    ...

## Level of service

#### Verification 

We ensure the email is legitimate and valid

#### Confirmation

We ensure the email belongs to the person who has subscribe

## Mode of service

#### Synchronous

You wait for Cruchot service confirmation to come back before letting your user in. It is fast and simple.

#### Asynchronous 

If you do not want to annoy your subscribers with a email confirmation flow, just
let them in. In the background Cruchot will verify their email and come back to you
to let you know if the user's email is valid so you can repudiate your users later on.
