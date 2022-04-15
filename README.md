TECHNICAL SPECIFICATION OF Go2

1. The purpose of the project

The goal of the project is to develop a Go2 application, the main purpose of which is to unite users interested in traveling together. In the application, the author will be able to monitor tourist points, and will receive full information about the situation in the selected city \ tourist point. Also, the author, in addition to being able to create and plan his entire journey in our application, he will also be able to describe his entire journey from A to Z in his personal posts in the same application. In addition, the application will have the possibility of correspondence between users - this will simplify the process of communication between users.

2. Application Description

The application consists of the following main functional blocks:
Registration, authentication and authorization
Functionality for the user 
Panel of countries that can be visited
Detailed description of the main tourist places on earth
A panel with the user's articles about the country he traveled to
Functionality for a full detailed description of the trip
Functionality for writing your own travel articles
Panel for finding travel partners
A panel with a personal profile where articles and travel directions are indicated


2.1. Types of users

The application provides two types of system users. 
First: The user creates articles and describes the best places during his trip, in turn, another user uses this information as a recommendation for making decisions and creating a template for his trip.
Second: The user is looking for a travel partner using our application.

2.2. Registration

One specific application installation is tied to one specific user. The system will most likely belong to Saas-type systems.
Thus, there will be no maintenance of different accounts under the type of Community / Society or company/organization at the moment.
The process of the author's establishment in the application will be implemented in the most usual way, and this is registration through the application. During the input of their data, the user will have to transmit the following data:
email — required field
password — required field
First and Last name - required field
The choice of 3 categories of interest is a mandatory field
Write about yourself - optional field
Write about previous trips - optional field
An important part of our application is the security of the user and his data, so for the provision we want to use the security system in it of the system. Also, for more accurate data security of those tourists who will use our application to search for travel partners, we will request more data. 

2.3. Authentication of the author and subscribers

Authentication of the author and subscribers is carried out by email and a one-time password (or a one-time link) that comes to this email (as implemented when logging into Skype from Microsoft).

2.4. Functionality for the user who will write articles

After authentication (login and password input), the user gets access to his personal profile in the System. The functionality for writing articles consists of the following blocks:
Text editing
Adding videos/pictures 
Establishment and content editing
Adding links and content
Establishment and editing of personal travel (History in Profile)
Mailing
Article analytics(number of views, support (likes), comments)

2.4.1. Functionality for the user who will be looking for a partner/partner

After authentication (login and password input), the user gets access to his personal profile in the Application. The functionality for a user who is looking for a partner / travel partner is generally very similar to Writing Articles, so it is important to mention here that a user who will be looking for a partner will have a certain level of security. 
The security levels will be divided into categories: Bright green - excellent, Yellow - good, Orange - not bad, Red - bad.

 

2.5. Profile Editing

In this section, the user has the ability to edit his profile data — email, adding a travel category, travel name, travel description, social networks. Possible social networks:
YouTube
Instagram
Facebook
VK
Linkedin
Twitch
It should be possible to change the password by confirming your old password.
If the user wants to change the style of colors, the application provides only two types of light and dark. 
If the application design implies some images for customizing the application page, then these images should also be edited from the author's profile.
2.6. Establishment and editing of personal travel (History in Profile)
For each trip, the following are set:
the name of the trip
, the description of the trip
, the cover of the trip
, the description of the total costs of the trip (optional)
adding photos (required)
Then the user will have the opportunity to switch from the Personal Travel tab (Stories in the profile) to articles written by users. It is important to mention that Personal Travel (Profile Stories) are divided into two types 1) Articles 2)Collecting photos from one trip.

2.7. Establishment and editing of content

The content published by the user can be formatted text with the possibility, at least, of highlighting the text in bold, italics, underlined, crossed out. It is worth adding the ability to create headers of different sizes for structuring long text content.
It should be possible to add lists and images to the content of the post, as well as the ability to attach files.
Each post should have a title.
It should be possible to create a teaser of the post — a cover and a description text about what is in this post. This teaser will be visible to guests (non-authenticated users of the System), as well as those whose subscription level is not enough to view the post.
Also, for each post, the subscription level at which this post can be read must be set. In addition to paid subscription levels, the subscription level "open to all" should be visible — such posts open to all will be visible to all users of the System, including guests who have not authenticated.(A CRAZY IDEA FOR A FUTURE APP)
It should also be possible to set a separate category for the post. That is, some posts may be visible only to those users who are interested in only one type of travel.
Parts of the post are the content itself and the teaser. A teaser is what is seen on the main page by both the one who has access to the post and the one who does not have access to the post. By clicking on the teaser, the post opens and the one who has access to the post.
The content itself can be inserted: formatted text (titles, bold, italicized, crossed-out text), images (downloaded from a computer), YouTube videos (shown in a standard built-in YouTube player), audio (downloaded from a computer, played in an audio player built into the System, only MP3 format is supported). It should also be possible to attach an arbitrary file downloaded from a computer — for subscribers it will be displayed as a link to download this file.
 
2.4.4. Setting and editing goals

The author can collect in the System for some purpose. To do this, he creates (and can edit later) a goal, within which he sets:
a description of the goal — a small text describing what the money is collected
for, the amount to be collected in rubles
On the public page, the goal is displayed with a description and current progress, for example, "107,775 out of 130,000 rubles collected"
There may be several goals. Payment for a goal is a one—time payment, not recurrent, that is, not debited monthly.(THE WORST IDEA FOR A FUTURE 
APPLICATION)

2.8. Mailing lists

The author can send mailings from the application.Basically, the user will be able to send posts, therefore, the editor is similar to what is used when creating posts, it is selected who to send the post to. You can choose several options, for example, in Whatsapp or Telegram.

2.9. Analytics

The author sees the following analytics:
Number of readers (one way or another number of subscribers)
Impressions
Coverage
Number of profile views
Click-throughs
Publications
References
Comments
Engagement
Like the article
 
3. Functionality for the reader (reader only)

The user can watch posts and like them, as well as increase their level of activity and engagement, thereby increasing their level of security (2.4.1). Comment under posts. Sharing posts is meant as a separate button — anyone who wants to share will do it by publishing a link. 
Each post can be added to favorites. In the favorites section, the subscriber should be able to create thematic lists. When adding a post to favorites, show these lists with checkboxes, at this moment the subscriber can immediately place the post in one of them.
Also, the subscriber should be able to edit his data on his profile page (email, change password) and cancel the Surveillance (subscription), which will stop the surveillance of the user.

3.1. Notifications about new posts
Automatically subscribers should receive notifications to their devices \E-mail about all new user posts in the application. Subscribers can cancel these and other emails by setting up in their profile.
 
4. Proposed technology stack

The following technology stack is proposed for the implementation of the system:

React Native - for cross-platform development.

For Internet acquiring, Tinkoff and CloudPayments are being considered, during the project it is necessary to compare the technical capabilities of the platforms and fees for payments. It is important to be able to pay with Google Pay and Apple Pay, including recurring payments (if Google Pay and Apple Pay allow you to do this, clarify during the project). It is important to open other countries in acquiring for the possibility of accepting payments not only from the Russian Federation, but also from CIS countries and other countries. Discuss this during the project with acquiring.
