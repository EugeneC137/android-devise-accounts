android-devise-accounts
=============
This is a little starter package for authenticating Android users with a Rails backend using Devise token authentication.  This was modeled after an article explaining how to setup token authentication on an existing devise project. http://matteomelani.wordpress.com/2011/10/17/authentication-for-mobile-devices/

This example never stores the user password on the system. It saves the authentication token given back by devise for future usage

Instructions
============
Setup your rails project to have an endpoint similar to this article: http://matteomelani.wordpress.com/2011/10/17/authentication-for-mobile-devices/.

Edit com.briangriffey.devise.auth.AuthenticationLoader and replace the localhost endpoint with your own endpoint.
If your service will return anything other than {"token" :token} edit AuthTokenParser to get the auth token from your response. 


Developed By
=============
Brian Griffey - brian@briangriffey.com


License
=============

      Copyright 2012 Brian Griffey
      
      Licensed under the Apache License, Version 2.0 (the "License");
      you may not use this file except in compliance with the License.
      You may obtain a copy of the License at
      
         http://www.apache.org/licenses/LICENSE-2.0
      
      Unless required by applicable law or agreed to in writing, software
      distributed under the License is distributed on an "AS IS" BASIS,
      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
      See the License for the specific language governing permissions and
      limitations under the License.