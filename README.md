# <img src="http://www.rice.edu/_images/rice-logo.jpg" width=180> Comp427, Spring 2018, Homework 1
## Rational Paranoia
The homework specifications, as well as the corresponding course slide decks,
can be found on the [Comp427 Piazza](https://piazza.com/class/jqifhp864b37ju).
This assignment is due **Thursday, January 17 at 6 p.m.**

You will do this homework by editing the _README.md_ file. It's in
[MarkDown format](https://guides.github.com/features/mastering-markdown/)
and will be rendered to beautiful HTML when you visit your GitHub repo.

## Student Information
Please also edit _README.md_ and replace your instructor's name and NetID with your own:

_Student name_: Nai-Fan Chen

_Student NetID_: nc41

Your NetID is typically your initials and a numeric digit. That's
what we need here.

_If you contacted us in advance and we approved a late submission,
please cut-and-paste the text from that email here._

## Problem 1
- Scenario: Stadium
- Assumptions:
  - You oversee the football stadium at a university whose team is frequently ranked among the best in the country.
  
- Assets:

  - The team members and fans are the most valuable assets in the stadium. 
  - The wallets in the fans’ pocket and their personal assets like camera.
  
- Threats:

  - If the bomb or weapons are taken into the stadium, it will hurt thousands of people who are watching the games. Nobody can prevent them from hurting people immediately because the police cannot use weapons in the crowd. That is, if they bring dangerous items into the stadium, tragedies will happen.
  
  - If the thieves hide in the group, they can steal the money easily since audiences focus on the game and they might not notice that the thieves are stealing their money. Moreover, the stadium will be very crowded, so it is difficult for the police to find the thieves since they can hide into the crowd and then pretend that they are normal fans.
  
- Countermeasures:
  - Do not allow to bring bags into stadium: bags can put lots of stuff into them and staffs could not check them all in short time since 50 thousand audiences (I assumed the capacity of the stadium is 50000.)  are not a small number. Although we can use the machine to scan every bags, it might also take much time and some special material cannot be detected. That is to say, if the items are wrapped into that special material, we cannot know what they are. On the other hand, if the fans cannot bring their bags into the stadium, although there is still a chance to take weapons, it will be less dangerous since the size of the weapons or bomb will be smaller and fire power will be limited. The police or audience can arrest the terrorists by hand.
  
  - Full-body scan before entering the stadium: this is one of the fastest ways to check all the audiences and staffs can make sure that they do not conceal dangerous items in their pockets. Hence, dangerous people cannot make damage or hurt people in the stadium without weapons.
  
  - Design evacuation route: If we cannot prevent tragedies, we need to evacuate people as soon as possible to minimize the losses. Every section needs to have multiple exits and have enough staffs to direct audiences to the nearest exit. Women and children might have higher priority to run out of the stadium because their movement will be slower than others’. However, if they evacuate at the same time, they will be left behind and be hurt by people behind them (they might be run over.). The space of the hallway is the biggest issue needed to be considered since if the capacity is not enough, lots of people will be stuck into the courts and hurt. Therefore, the evacuation route(shortest path to the exits) and space of the corridor are significant features to reduce the damage and losses. 
  
  -	Warning sign: Put the signs in front of every seat to make people notice the thieves. By doing so, people will put their wallet into a safe place and look around to find out whether there is a suspicious person nearby. Hence, it is difficult for thieves to steal money from our fans. 
  
## Problem 2
- Scenario: Documents

- Assumptions:

  - As head of IT for an international law firm, you are responsible for a document management system; some documents stored there are about sensitive legal, financial, or political matters.
  
- Assets:

  - Documents: sensitive legal, financial or political matters.
  
- Threats:

  - Hackers can hack in and steal the documentation if they know how to break the firewall. If they sell this information to the newspaper publisher or other people who would like to take advantage of it, the company will bankrupt very soon because nobody will trust our company.

- Countermeasures:

  - Data mask: change content (like name, address, …) of the data, so our customers or users (staffs, engineers) will not see the real information. That is, the sensitive information of every lawsuit will be covered. For example, the owner of the file is ‘John’. The data mask algorithm will turn ‘John’ into ‘Eddie’. By doing so, no one will know who is the real owner. This can also be applied to other columns as well. If these masked data leaks out, we do not need to worry about our customers’ privacy. Although the hacker can get our information, the original one still saves in the safe place. Moreover, the masked data is not reversible, so the hackers cannot get the original one by decoding.
  
  - Separate the data and store in different servers: If we can separate our data and distributed to many servers, the hackers can just get some parts of our data instead of all of them. The hackers can just get the incomplete files if they just cracker one of our servers and it is almost impossible to break them all. Moreover, the files are everywhere, so it is difficult to locate the certain files they want. Therefore, building a great hash function to distribute the files to different machines will make our files harder to be accessed. 

## Problem 3
- Scenario: Facebook

- Assumptions:

  - Facebook is the biggest social network company. The users have connected with their friends and chat with each other very often. Furthermore, Facebook also collect data from their users such as where they are at certain time slot, or what topics of passages they are interested in.
  
- Assets:

  - Personal information like education, work, etc.
  - The post and friend connections.
  
- Threats:

  - In Facebook, users can share their activities with other people who follow them or chat with their friends in real time. If hackers can log into certain accounts that do not belong to them, they can spread virus through Facebook messages or posts. For example, they can post a link (or send it by message) that contains virus and account owners’ friends who trust them and click the link without doubt. The virus will spread very soon since users on the Facebook usually have hundreds or thousands friend connections or followers.
  
  - The database system might leak the users’ information such as their name, where they had been, what their jobs are and so on. The valuable information might be stolen and sell it to advertisers. That is, the company will lose lots of money and will also have lawsuit regarding privacy issue.
  
- Countermeasures:

  - Device or browser detection: when the new browser send the new login request,  we will send the email or SMS to the default address or phone number to confirm whether the user really send the request. If we cannot receive the confirmation, the system will frozen account until the account owners change the password.
  
  - Login IP detection:  If the account owner is living in USA, but someone login in Europe. This might not the account owner, but the hackers try to break the password and get the information. The system needs to detect this abnormal IP address and send the abnormal login to the account default email and deny the login until the owner accept.
  
  - Two-step verification: The code generator will change the code every minute. Every time someone would like to login, they will ask the code. This code is hard to get because it changes all the time, so even if there are some people can get the code, the code will expire very soon. Thus, it is hard to login if people do not get the code generator.

