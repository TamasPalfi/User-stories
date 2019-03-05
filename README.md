# What is Members Only?

Members Only is a social media site where users, known as Members, can post statuses, photos, links, and everything else that one may post on another social media outlet. So what makes us different you may ask? Exclusivity. Not just anyone can join Members Only. You have to receive an invitation from another Member or be lucky enough to get an entrance code from one of our Idols. This makes Members Only a gated community, where we can house exactly the people that we want to be on the site. This is formulated and handpicked data, which can, and will, be used for a multitude of profitable purposes. 

# The Pillars of Members Only

## Members

Members are our users. They are the the traffick, the data, and most importantly; the revenue. Members are able to access the site via a login page that brings them to their feed, where by default they are connected with every other Member on the site. This allows them to see the statuses, photos, and anything other form of output from every other Member on the site. Otherwise, Members have the option to privatize their profile so that they can only be seen by their followers (other Members who either invited this Member or were invited by this Member). But the most important question is, what do Members bring? The answer is: data. And heaps of it. We plan to store all of Members posts, comments, photos, filtered photos, the time they spend on certain areas of the site, what statuses and links draw their attention, and anything else imaginable. All of this knowledge will allow us to carefully curate advertisements for each individual user as to draw the most potential revenue to the site. And for all their actions on the site, we reward Members with points. A simple mechanism that will keep Members wanting to keep coming back to the site. They post a photo and filter it? Have some points. They post a status that receives a lot of comments? Have some points. A Member successfully gets a new Member to join the site? Have some points. And with these points, Members can choose to use them to invite new Members to the site, expanding their circle of friends within the gated community. This allows Members to create subcommunities within the overarching Members Only site, which will keep Members entranced with the website. Without Members, Members Only doesn't exist. 

## Idols

Idols are our bedrock from which we build the site. We will pay Idols to be some of the first enhanced Members on the site. Enhanced meaning that they have all the functionality of a normal Member, but they also have unlimited points and invitation codes which they can use to send invitations to Members Only to all of their fans. In this sense, Idols are the first step in attracting large waves of Members to join the site and get it off the ground. Once on the site, Members can see all of their idols updates, effectively joining the community of the Idols. 

## Administrators

Administrators are our next enhanced Member. First and foremost, we have admins to keep the peace. Admins will manually review any flagged content to make sure that no illicit material makes it on to Members Only. Although Members Only is a gated community, we do not want to establish a reputation for allowing unlawful material on our site. Furthermore, admins will solve disputes between Members, effectively making sure that our Members are happy on the site. Finally, admins will be able to insert sponsored content and different filters into other Members photos as to please advertisers of the site. Additionally, administrators will be able to add links, comments, and other materials into Members posts for advertising and any other purposes of the site. And of course, the original poster will not be able to see the changes that were made to their posts, but everyone else on the site will be able to. 

# User Stories

<details>
<summary>New Members</summary>
 
### 1. New Member Creates Account

Josh gets sent a link from a friend to join Members Only. Naturally, Josh is very excited and is eager to join the site. Josh finds the link in an email from Members Only and selects it. He is now brought to a Members Only webpage that asks him to confirm if he wants to join Members Only. Josh will of course select yes on joining Members Only. After accepting, he will be brought to a Sign Up page on the website. Josh will have to fill out a form will personal information such as First Name, Last Name, Street Address, City/Town, Zip Code, Country (U.S. only to start), Email Address, and a Password. Josh will then select a box which says that he accepts the Terms and Conditions of Members Only. Finally, Josh will submit this form, and he will be sent a confirmation email about joining Members Only. Josh will go to this email, select the account confirmation link, effectively finalizing the creation of his account and bringing him to his own Members Only account. Afterwards, Josh will be sent a credit card charge that he will have to verify on the site to confirm that he says he is. 
 - Non-Functional Aspects:
   - Web Server receives form submission
   - Web Server sends to Node.js backend
   - Node.js backend sends automated email
   - Member's data get sends to database through interface calls

### 2. Signing Up With a Code

Brianna manages to get her hands on an invitation code to Members Only from one of her favorite idols. To use this, Brianna navigates to the Members Only site and is brought to the login page. Since Brianna doesn’t currently have an account, she will have to choose the option to sign up with a code. After clicking this, Brianna will be brought to a new web page where she will be asked to enter her code. Brianna will enter the code and then hit a submit button. Afterwards, she will be brought through the same account creation process as described previously. 
 - Non-Functional Aspects:
   - Web Server receives form submission
   - Web Server sends to Node.js backend
   - Node.js backend sends automated email
   - Member's data get sends to database through interface calls

### 3. New Member Invitation Link Expires

Liam receives an invitation link to Members Only. However, he is very busy and forgets to about it for more than 4 days. Because of this, the email link will expire, and he will lose this opportunity to join the site. To be able to join again he will have to be sent another invitation link. 
 - Non-Functional Aspects:
   - Node.js backend keeps track of how long unnaccepted invitation has been sent out
   - Node.js backend terminates validity of invitation instance

### 4. New Member Confirms Credit Card Charges
After successfully creating her account, Catherine will have to enter her credit card details so that we can confirm she is who she says she is. Catherine will receive an email to confirm her payment details. Catherine will select this link which will bring her to a form on the Members Only site where she will enter a valid 16-digit credit card number, the name the card is under, the expiration date of the card, and the 3 digit CVV associated with the credit. Catherine will then choose to SUBMIT this form. She will then be brought back to her Members Only page. 
 - Non-Functional Aspects:
   - Web Server receives form submission
   - Web Server sends to Node.js backend
   - Member's data get sends to database through interface calls

### 5. New Member Confirms Credit Card Charge

After Catherine successfully enters her credit card information, she will be charged a random amount between $0.20 and $0.45 that she will need to confirm on the Members Only site to verify she is who she says she is. Catherine will receive an email shortly after creating her account that notifies her that she has been charged for the first time. Catherine will then navigate to her online banking and check for a charge from Members Only. After finding the charge, Catherine will remember the amount and navigate back to notification email from Members Only. Catherine will select the hyperlink in the email that brings her to a form with an entry field for the value of the charge. Catherine will then enter the charge amount and select SUBMIT. If she submits the correct amount then she is brought back to her Members Only page as a verified Member. Else, she will be asked to resubmit the amount she was charged until she submits the right amount. 
 - Non-Functional Aspects:
   - Node.js backend sends automated credit card charge using Stripe.js
   - Web Server receives charge amount input
   - Node.js receives input and validates it is the same as amount charged



</details>


<details>
<summary>Members</summary>
  
### 6. Member updates credit card information

Alex will login to their profile. Alex will navigate to their settings page on their personal profile. Member will choose change credit card button. System will prompt user with text boxes to enter new credit card information. User will enter name of card. User will enter card number. User will enter expiration date. User will enter CVV. Alex will hit the submit form button. Credit card will then be verified to make sure it is valid. System will send this to the database to update the current credit card information with this information. Credit card information updates.
 - Non-Functional Aspects:
   - Web Server receives form submission
   - Web Server sends to Node.js backend
   - Node.js backend accesses database through interface calls to update information associated with particular Member

### 7. Member Confirms Tri-Monthly Credit Card Charge

System will tell the credit card software it is time to charge Alex. Credit card system will charge member a random amount between $0.20 and $0.40. System will send automated email at specified time period telling member to validate the charge made to their account. Email will include a link that will direct the user to the page to enter the amount charged. System will start a timer for 3 days. Alex will login to their personal bank account and check for the charge from Members Only. Alex will click link provided in email. Alex will be redirected to the webpage with a form where they can enter the amount they were charged by the system. Alex will fill in the text box with that amount. Alex will hit the “Submit form” button. Webserver will receive this information and back end services will process it. System will compare this amount to the amount that was charged. If right, member will be directed back to the Members Only home page. If wrong, member will be blocked out of Members Only until they enter the right amount.
- Non-Functional Aspects:
   - Node.js backend sends automated credit card charge using Stripe.js
   - Web Server receives charge amount input
   - Node.js receives input and validates it is the same as amount charged

### 8. Member does not enter the amount in time

Alex doesn’t enter amount in time and is blocked from account. When Alex tries to access Members Only, they will be directed to a page telling them to send another charge. System tells credit card system to send another charge between $0.20 and $0.45. Credits card system sends another random charge. System sends Alex another email. System starts a timer for 3 days. Alex logs into their bank account and sees the charge from Members Only. Alex clicks button on email and is redirected to Members Only. Alex enters amount in and is either allowed back to website or entered the wrong amount.
- Non-Functional Aspects:
   - Node.js backend sends automated credit card charge using Stripe.js
   - Web Server receives charge amount input
   - Node.js receives input and validates it is the same as amount charged

### 9. Member posts a status update on personal profile.

Alex will click an option on their profile page that reads “create new post”. Alex will type URL, and can add any additional text to the post. tinyURL generator will shorten the URL given. Alex will hit “post”. The webserver will receive the request send it to the backend. Backend will process the request and post Alex link to their profile feed. Backend services will send the link to the database to store it as something Alex is interested in for potential future advertisement reasons.
- Non-Functional Aspects:
   - Web Server receives new post
   - Node.js backend receives post information and posts it
   - Node.js backend uses database interface to update post table with new post 

### 10. Member leaves comment on friend’s status.

Alex will see their friend’s status on their profile feed. Alex will click the comment button that appears on the bottom of their friend’s post. The Webserver will get the request and pop up a text box overlay on the website. Alex will leave a comment, then hit “Post”. The Webserver will receive the request and send it to the backend services. Backend services will add it to the friend’s comment section on their post.
- Non-functional Aspects:
   - Web Server receives new post
   - Node.js backend receives comment information and posts it
   - Node.js backend uses database interface to update comment table with new post 

### 11. Member invites a non-member to Members Only so that they can enjoy Members Only with them

Alex navigates to the “Invite New Member” button on their profile page. On this page, Alex will fill in new members email address. Webserver will receive this information and pass it to the backend. Backend will save new members email to database. Backend will tell email system to send a new invitation email. New invitation email will be sent to new member. System will start a timer for 4 days.
- Non-functional Aspects
   - Web Server receives request to send a new invitation link
   - Node.js backend processes request and sends an automated email with link
   - Node.js backend keeps track of how long invitation has been out for

### 12. New Member Accepts Offer

Alex will gain points. Webserver will receive this information and send it to the backend. Backend will add that many points to Alex’s point system.
- Non-functional Aspects:
   - Web Server receives new post
   - Node.js backend receives post information and posts it
   - Node.js backend uses database interface to update post table with new post 

### 13. Member posts photo to profile.

Alex will choose “Post Photo” on their profile feed. Alex can navigate their device for the photo they wish to submit. Alex can then add any additional text to the post that they wish. Alex will then hit submit. The Web Server will receive the request and send it to backend services. Backend services will process and post the request. Backend will save image to database. Admins can use saved image for their own purposes.
- Non-functional Aspects:
   - Web Server receives new post and photo
   - Node.js backend receives post information and posts it
   - Node.js backend uses database interface to update post table with new post
   - Node.js backend uses database interface to update photo table with new photo

### 14. Member removes/applies filter to photo.  

Alex will go through the post a photo process, except immediately after he chooses his photo he will be given the option to apply a filter. Alex will scroll through various premade filters available on Members Only. Alex will choose a filter that will be applied to their photo. The post photo process then continues from here.
- Non-functional Aspects:
   - Web Server receives new post and photo
   - Node.js backend receives post information and posts it
   - Node.js backend uses database interface to update post table with new post 
   - Node.js backend uses database interface to update photo table with new photo
   - Node.js backend uses database interface to update filtered photo table with new photo

### 15. Member removes filter

Alex navigates to his profile page and clicks on the photo he wishes to remove the filter on. Alex chooses “options”. Alex then chooses to remove filters. The filters will then be removed from the photo. Alex will then be prompted to confirm their changes. Alex will click “Confirm”. Request will be sent to the web server. Web server will send it to backend. Backend services will replace that photo with the originally posted photo.
- Non-functional Aspects:
   - Web Server receives new post and photo
   - Node.js backend receives post information and posts it
   - Node.js backend uses database interface to update post table with new post 
   - Node.js backend uses database interface to update photo table with new photo
   - Node.js backend uses database interface to update filtered photo table with new photo


### 16. Member Adds Sponsored Content

Alex will follow the posting photos process. Alex will then click add content. Alex can choose any of the items and place them anywhere in their photo using a drag and drop method. Alex will choose to submit their altered photo. The Web Server will receive the request and send it to backend services. Backend services will process and post the request. Backend will save image to database. Admins can access image and add/delete content as they please.
- Non-functional Aspects:
   - Web Server receives new post and photo
   - Node.js backend receives post information and posts it
   - Node.js backend uses database interface to update post table with new post 
   - Node.js backend uses database interface to update photo table with new photo
   - Node.js backend uses database interface to update filtered photo table with new photo

### 17. Member Removes Sponsored Content

Alex will go to their photo with added content. Alex will select options and be given an option to remove content from the photo. Alex will be shown what is added content in their photo such that they can navigate to it and choose to remove it. Alex will submit their changes. The Web Server will receive the request and send it to backend services. Backend services will process and post the request. Backend services will save image to the database. Admins can use image to add/remove/etc. Original poster will not be able to see these changes. 
- Non-functional Aspects:
   - Web Server receives new post and photo
   - Node.js backend receives post information and posts it
   - Node.js backend uses database interface to update post table with new post 
   - Node.js backend uses database interface to update photo table with new photo
   - Node.js backend uses database interface to update filtered photo table with new photo

### 18. Member Logs in to Members Only

Johnson wants to login in to Members Only and check his feed. To do this, Johnson will navigate to the Members Only homepage, which includes a login for existing users form. Johnson will enter his email address and password associated with his Members Only account. Johnson will then select LOGIN at the bottom of the form. If his email and password are correct, he will then be redirected to his Members Only feed. 
- Non-functional Aspects:
   - Web Server receives form submission
   - Node.js backend receives login request and validates credentials

### 19. Member Forgets Password or Inputs Invalid Password

Johnson wants to login to Members Only, but he is stuck at the login form on the homepage of the site because he has forgotten the correct password associated with his account. Johnson will then select a link that says, “Forgot Password”. This will redirect him to a different form on the Members Only site where he will fill out his email and several other details associated with his account such as his name. Johnson will then be sent an email that sends him a new temporary password to login to his account. Johnson can then reset his password once he logs back into his account and accesses his settings. 
- Non-functional Aspects:
   - Web Server receives form submission
   - Node.js backend receives login request and rejects credentials

### 20. Member Forgets Email or Inputs Invalid Email

Johnson directs himself to the Members Only homepage and tries to login to his account. However, Johnson has somehow forgotten the email associated with his Members Only account. After entering his information, Johnson will click submit. The system will receive the email and attempt to verify who Johnson is, however because it is the incorrect email Johnson will be denied access to Members Only until he can recall the correct email address associated with his account. 
- Non-functional Aspects:
   - Web Server receives form submission
   - Node.js backend receives login request and rejects credentials

### 21. Member Changes Password

Larry wants to change his password, either for security reasons or because he just logged in with a temporary password because he forgot his previous one. Larry will navigate to the SETTINGS portion of his account after immediately logging in. Larry will then navigate and choose the CHANGE PASSWORD option. Larry will be brought to a separate, private form where he will be prompted to enter a new password. After entering the new password, Larry will be prompted to enter it a second time as to confirm the password and eliminate the possibility of any typos. Larry will then click CONFIRM and the system will verify that the passwords are identical. If they are, then Larry will be redirected back to his Members Only feed. Otherwise, Larry will be prompted to enter and reenter the new password again until he successfully enters the same password twice. 
- Non-functional Aspects:
   - Web Server receives form submission
   - Node.js backend receives new password
   - Node.js uses database interface to update values associated with Member

### 22. Member Changes Visibility Settings 

Danny wants to hide his activity from non-followers on Members Only. To do this, Danny will go to his personal page and access the SETTINGS portion of the page. Danny will then navigate to the toggle button which allows them to switch between a privatized and un-privatized profile. Since Danny wants to privatize his page, he will select this toggle button to the on setting, effectively hiding his activity from non-followers. 
- Non-functional Aspects:
   - Web Server receives change of privacy request
   - Node.js backend receives request
   - Node.js uses database interface to update values associated with Member

### 23. Member Blocks a Follower

Syed wants to block one of his followers that ruining his experience on Members Only. Syed will go to their Members Only personal page. Syed will then go to their followers list and navigate to the person they are concerned about. Syed will then choose to block this follower, which will disallow them from seeing any of Syed’s information, status updates, posted pictures, or any of Syed’s activities on the site. 
- Non-functional Aspects:
   - Web Server receives block request
   - Node.js backend receives block request
   - Node.js uses blocks data communication between these two Members

### 24. Member Reports Another Member

Phil wants to report another member on Members Only for an offensive action. Phil will go to his personal page and access his followers list, navigating to the person he is concerned with. Phil will then choose the option to report this follower. Phil will then be redirected to a report issue page that contains a form where he will enter the member’s name he is concerned with and other details about why they are being reported. After filling out the form, Phil will click SUBMIT, sending the form to the Web Server. This information will then be redirected to Admins so that they can review the report and decide any further action. 
- Non-functional Aspects:
   - Web Server receives block request
   - Node.js backend receives block request
   - Node.js uses blocks data communication between these two Members
   - Node.js sends report to Admins

</details>


<details>
<summary>Admin</summary>

### 25. Administrator Removes Member's Access to Member's Only
Administrator Ava is working through checking the flagged content on the Member’s Only site, and she encounters the profile of Jonas (a member) who was flagged for posting inappropriate content.  Ava directs herself to view Jonas’s profile via frontend interactions.  From there, she must review all the flagged content on his profile and come to a decision on whether Jonas should be removed or not from Member’s Only.  Ava concludes that Jonas must be removed for violating the site’s posting policy.  She selects the “Remove Member” button via the webpage which should then cause a confirmation pop-up to occur.  Ava selects the “Yes” option which causes the web server to receive that request and send the needed backend services to comply with that order.  The backend removes Jonas as a member by effectively deleting the profile page and all associated comments with the profile, but the personal data is retained.  
- Non-functional Aspects:
   - Web Server receives removal request
   - Node.js backend receives removal request
   - Node.js disallows Member's credentials to be used to login

### 26. Administrator Removes Content Flagged as Inappropriate/Illegal
Administrator Ava is working through checking the flagged content on the Member’s Only site when she receives a report of inappropriate content in the form of a flagged photo.  Ava directs herself to review the flagged photo via frontend interactions, and she must come to a decision on whether the photo should be removed or not.  After noticing that the photo does indeed contain child pornography images on it, Ava proceeds with removing the photo.  She selects the “Remove Post/Photo” button on the web page which would cause a confirmation pop-up to occur.  After selecting the “Yes” button, the web server receives that request to remove post and directs it to the backend.  The backend then removes the flagged photo from the page AND the database (no need to keep flagged data).  
- Non-functional Aspects:
   - Web Server receives removal request
   - Node.js backend receives removal request
   - Node.js uses database interface to remove data from the site

### 27. Administrator Edits Member's Photo
Administrator Andrew wants to make Member’s Only the best visually pleasing web-page out there.  Thus, he decides he wants to edit a member’s photo to add a filter in the hopes that it would increase web traffic to the site.  First, Andrew directs the web page via frontend interactions to the photo on Curtis’s (a member) profile that he would like to edit. Andrew selects the “Edit” button next to the photo, and he uses the photo editing software to apply a color filter.  After making the necessary revisions, he selects the “Save” button which would cause a confirmation pop-up to occur.  Andrew confirms he’s satisfied with the changes by selecting the “Yes” button.  The web server gets this request to save and sends it to the backend.  The backend then saves this new photo to the database as well without removing the original photo.  However, the filter has been added and the photo is updated correctly.  Adding filters is not the only thing that Andrew can do to Curtis’s photo. He could also choose to add sponsored content which he would do to also increase web traffic and revenue in terms of partnerships.  The process Andrew take to do that is nearly identical to the filtering case except Andrew uses the photo editing software to input another image (the sponsored content) onto the photo rather than apply a filter.  It’s also important to note that these two interactions described above could very well occur as or in a comment instead of a post.  This is as simple as just a different location where Andrew is working to change content from.  A final comment is that visibility does have an effect here, as Curtis would not see the changed content on his own profile but rather what he originally posted.
- Non-functional Aspects:
   - Web Server receives new post and photo
   - Node.js backend receives post information and posts it
   - Node.js backend uses database interface to update post table with new post 
   - Node.js backend uses database interface to update photo table with new photo
   - Node.js backend uses database interface to update filtered photo table with new photo

</details>



<details>
<summary>Idol</summary>

### 28. Idol Has All Privileges of a Member
Tony loves using Member’s Only, and as a popular social figure he has the designation from the Member’s Only site as an idol.  That basically grants him additional capabilities on the site outside of what a normal member can do such as unlimited invitations and ability to post sponsored content.  However, it is important to remember the fact that Tony still is essentially a member.  Thus, as such, he can do all the basic functionally that a member does such as posting a status update, commenting, posting a photo, and applying filters to photos.

### 29. Idol Invites a New Member
Tony, an idol, wants to contribute to the web site’s overall member base count by inviting new members to the site.  He does this to increase the web traffic to Member’s Only and increase his own revenue.  There are two ways an idol can send invitations; the normal way for most members which is through an email invitation or via code referral.  To send via email invitation link, Tony selects the “Send Invitation Link” button on the web page.  He enters the email address of his friend Bruce which is bruce4321@gmail.com, and the system confirms that it is a valid email address. It is in fact a valid email address, so Tony selects the “Confirm” button to send the invitation link.  It’s important to note here that as an idol, Tony has unlimited number of invitations, so he doesn’t get docked any points upon inviting his friend.  The next way of inviting is through the code system.  Tony will generate a random, new invitation code which will be suitable for one invitation only.  Tony can then give this code out through a variety of means either through person, message, Facebook, or any other communication means.  Whoever receives this code from Tony, then must use it when signing up for Member’s Only.
- Non-functional Aspects
   - Web Server receives request to send a new invitation link
   - Node.js backend processes request and sends an automated email with link
   - Node.js backend keeps track of how long invitation has been out for

### 30. Idol's Visibility
Since idols are the “Popular” faces of Member’ Only, we want it to be the case that all members should be allowed to see their profiles. Thus, idols don’t have the visibility toggle option as a part of their profile allowing all members to be able to follow their profile.  This differs from regular members in which they can toggle their visibility of their profile from specific members.  
</details>


<details>
<summary>System</summary>
 
### 31. System Deducts Points From Member  
The backend receives a request from the frontend. The backend sent a request to the credit card company using a credit card software.
If the credit card is denied, the system freezes the member’s account and changes the permission of the member in a database. 
If the request is successful, the database finds the matched member and takes a point off. Then the system sends updated point information to the frontend. The frontend updates the point information in a local storage and Alex will recoginize the changes.

### 32. System Awards Points To Member  
Alex’s invitation gets accepted or he makes positive actions. The backend receives a request. The database finds the matched member information in a database and updates the matched member's information. The system sends updated point information to the frontend. The system updates the point information in a local storage and Alex will recognize the changes. 

### 33. System Receives Login Request From Frontend 
A frontend sends a login request to a backend. The backend gets a request that contains user information. The backend stores a member's current IP address into the database. The backend confirms whether the information given is matched with one of the user data in the database. The backend sends tokens and matched user information to the frontend. 

### 34. System receives Logout Request From Frontend   
 Alex clicks a logout button in a frontend. The frontend detects when the logout button is clicked. The frontend sends a Alex’s singed out time to a backend. The backend stores Alex's logout time. The frontend destroys the session data in a local storage. The frontend redirects Alex to a landing page. 

### 35. System Receives Registration Request From Frontend 
A potential member(Bob) fills out a registration form and clicks the register button. The backend gets a request that contains a potential user’s information 
If the credit card information already exists, the backend sends an error to the frontend  and bob checks the error . If the credit card information does not exist in the database, The system checks the given credit card information is valid using credit card software. If the data is valid, the system stores new user information into the database. The frontend redirects Bob to a login page. 
If the data is NOT valid, the backend sends an error to the frontend and Bob checks the error. 

### 36. System Retains Member's Actions (Interests)
Alex performs specific expected actions. The frontend detects an item being clicked when a member clicks a specific post or recognizes an item(content) on the current screen (if a member stays longer than a particular second at the same page without scrolling down or going out to other pages). The frontend sends the item(content) information to the backend. The backend receives the data and stores them in the database.

### 37. System Converts URL to Shortened URL 
The frontend sends the request to a backend. Then the frontend sends a request to the backend with original URL information. The backend gets the request and uses a hash function to generate a shortened URL. The system saves the shortened URL into the database. The system sends the shortened URL to the frontend. In the case of the system can't perform shortening, it will use the original URL. 
</details>
