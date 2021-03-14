# Wysa-Backend-Developer
Question 1 .

The signup phase of the application will look like the following : 

$.ajax{(
url : 'signup/api/user',
method : 'POST',
data : {nickname : nickname , password : password},
success : function(data){
if err : console.error
else : redirect to 'home/api/start'

} 

)}

User Signup -> Optional user signup auth using google

<<<<
Application Type: Web Application
Authorized Javascript origins: http://localhost:8080
Authorized redirect URI: http://localhost:8080/auth/google/callback
Copy and paste Client ID and Client secret keys into .env


>>>>

Backend(For User Registration):
  //Check if user exists :
  User.findOne({nickname : req.body.nickname})
        if exists : res.status(400) {User exists}
        else: new User({"nickname", "password"})
  Hash Password for Mongo 
  
  // Hash the password using bcrypt 
  bcrypt.genSalt((err,salt)=>{
    newUser.pass= hash
    newUser.save()
    .then(user => res.json(user))
  
  
  })

----------------> Move Forward to the onboarding phase : 
FOR A WEB API A GOOD DESIGN WOULD BE TO HANDLE THE ONBOARING PHASE FOR EACH PROCESS i.e :


 1. Sleep 
 2. Anxiety 
 3. Depression
 
 
 "home/api/start" with a single FORM based approach . 
 This is done to keep the hassle of session change to a minimum 
 But for a design mentioned in the example 
 
 onClick event will be fired for example :
 
 
 onClick GET : Every category handles different initial question phase
 
 if onClick(category == 'SLEEP'){
    "home/api/start/:categoryID"
 }
 redirect to "home/api/start/:categoryID/"
 
 form details with required questions : 
 
" That's a great goal. How long have you been struggling with sleep "
" How many hours do you get ? " 
 
----> POST request : 
    {
    url :'home/api/start/:categoryID/',
    method : 'POST',
    data = { sleep : sleep ,time : time , bedTime : bedTime, nightSleep : nightSleep }
    success : function(data){
    
    check for errors 
    redirect to corresponding plan for the user
    }
    }
 
 
------> Database Handle 

Handling the data for the user with a particular entry for every with nickname as primary key.




Database : 
User Table : {username : Shaurya, password : *****, fname : Shaurya, lname : Sharma, category : ["sleep","depression"]} 
Onboarding Plan : {sleep : '2 to 6 weeks' , time : '1:00' .... }


The time and string variables need to be handled differently to avoid date formatting errors.

---> Redirect User to the upcoming homepage for Premium or Free Plan change.

 
 
  _____________
 |  Sleep
 |  Anxiety
 |  Depression
 |
 
 
 


