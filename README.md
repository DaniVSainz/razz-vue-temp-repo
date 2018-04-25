# razz-vue-temp-repo

Razz Vue Rewards 

### Notes
1. There's a lot of stuff that I would have liked to do however I just could not afford to invest more time into the challenge.
2. I had a lot of fun having an excuse to try out Vue and was impressed by its similarities with other frameworks.
3. I would have liked implementing a ticket system for the rewards with a job that processes them in order until out of stock however I  did not have time for it.
4. I also would have liked to make it pixel perfect and more responsive however I could not afford to invest that amount of time into it.  

### Online at https://razzvuerewards.herokuapp.com/  
1. Since im using a free Gmail account to send out emails sometimes there can be issues using it on prod with delayed emails 10+min or google triggering security measures requiring manual intervention.
2. Because of this I setup registration on the front and back to log you in automatically, however upon logging out and back in you will be prompted
to verify your email via the link sent out to your email.
3. For your convenience, there's a seedDB button in the top right dropdown that drops the Prizes collection and reinserts documents.




### To run in dev you need a .env file in the root of the node-backend folder.
Feel free to use the razzvuerewards email i sent to Kenney, however, I cannot guarantee that Google won't flag the different ip requiring me to unlock the account.  
  
 .env File formatting  
userEmail=  
userPass=  
mongoUrl=mongodb://localhost:27017/vue-redeemExpTest  
secret=yoursecret  

### Dev notes  
Emails in dev are sent with a https link, if you're running in http they will not work and you'll have to remove the s to test the links.  
### There's two ways to run the project  
1. cd into client & npm run dev.Then in another terminal cd into node-backend & nodemon/node bin/www. Client would run on localhost 8080 and backend on localhost:3000
2. Or cd into node-backend & npm run startDev . This would serve our frontend bundled ontop of the express backend.
