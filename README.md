# SGF Web Devs Mobile App

## Concepts

- Sign In Screen 
	- Potential auth ideas
		- Github
		- Meetup
		- Or general social and or email


- Feed
	- Live list of who has checked in
	- Details about the evening pulled from Meetup
		- Niceties
			- In the future the desire is to click through to individuals and learn more about them. What kind of dev work they do, what meetings they have been to, etc. This may/may not play into some of the decision making on authentication.


- Checkin
	- Once checkin button is tapped, user is reflected in the live list and is eligible to win a prize for the night
	- Niceties
		- Show Map
		- Pull event details from Meetup
		- Cross reference geolocation point to be within a mile radius of address from meetup to ensure the user is at the event
		- Do all things possible to prevent checkin abuse


- Raffle system
	- This will be the portal where a Web Devs host will control what is being given away for the night and press a button to automate a random drawing from the list of attendees who have checked in.
		- Example
			- 2 Pluralsight trials
			- 1 Jetbtains license
			- 3 Telerik TShirts
	- This will send a push notification to each user alerting them that they have won.
		- The UI that the user sees should have a couple different items on the screen
			- Title and description 
				- For giveaways that require an email address
					- A pre-filled email input for user to verify that is their email or the email they wish to have the item sent to
					- 	A confirm button
	- Niceties
		- A real time displays on the admin side so that it can be projected on the screen for everyone to see while the drawing is happening.
		- A pass button that the user can press to pass on the prize. This happens sometimes when the user might already have what he/she has just won. Or maybe they have no interest in the item.


## Technologies

Since this is a group effort, it would be ideal to stick to a primarily web based toolset. At the moment Ionic combined with Firebase feel like a pretty good mixture to handle most everything needed for the scope above. Firebase offers real-time data out of the box as well as many other features. Ionic is essentially a skinned up version of Cordova with a robust Angular underpinning.

The floor is open for suggestions, though. If anyone has success stories with using other technologies we would love to hear them!