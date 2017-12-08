# Chapter 5: Networking and the Internet
(Completion Time: 3 Weeks)

## Central Focus
Students will transition from programs that exist only on their IDE to programs that can be viewed globally. They will explore the global system of interconnected computer networks that use the Internet protocol suite (TCP/IP) to link devices worldwide and the languages which enable them to express their ideas on the internet.

---

## a. Internet Basics
_An overview of how the internet works and how we as users interact with it. This topic can also be used as sort of a teaser for the rest of the chapter._

### How to Launch the Lesson:
Have students write down their ideas of how they think the internet works. Revisit these ideas at the end of this chapter. What was correct? What was incorrect? What do students still have questions about?

---

## b. IP Addresses
_IP (Internet Protocol) addresses are assigned to each device connected to a network. A device or web page can be identified by its IP addresses, as all are unique - like a postal address._

### How to Launch the Lesson:
Have students find their IP addresses. Why does everyone on the internet need a unique IP address? Students can switch IP addresses with peers and try to track the location using http://what-is-my-address-ip.com/ or a similar site.

#### Activity: Your IP Address
Have students find their IP addresses on their computer and connect to one another's addresses using the terminal command ping or something similar.

#### Activity: Your Favorite IP Address
Have students find the IP addresses of their favorite websites and get to them by typing the IP address instead of the URL.

---

## c. DNS and DHCP
_DHCP, also known as the Dynamic Host Configuration Protocol, dynamically assigns IP addresses to devices connecting to a network. DNS, the Domain Name System, is responsible for translating URLs of websites to IP addresses and vice versa. We need both IP addresses to be able to form a successful connection from sender to receiver._

### How to Launch the Lesson:
Have students think of metaphors that represent the roles that DHCP and DNS play with regards to IP addresses. Would it still be able to access websites without DHCP? or DNS? Are both necessary?

#### Demo: Phone Book
An analogy for DNS to use is a phone book - you look up a person's name, and are given their phone number if you need to contact them. This is similar to typing in a website URL, which is then translated to an IP address.

#### Demo: Dynamically Assigning Numbers
An analogy for DHCP could be anything dealing with dynamically assigning numbers to devices, i.e. numbers at a deli, characters in a board game, etc. The key is that it is possible to have the same number more than once, but that it is not guaranteed.

---

## d. Routers
_Routers are the components of the Internet that direct packages of data across various networks. They follow a set of rules to direct packets based upon IP address and port. Typically routers will direct individual packets on different routes to end up at the same location._

### How to Launch the Lesson:
Let each student pick a unique website. Then use a site similar to http://www.yougetsignal.com/tools/visual-tracert/ to view the trace route for each site or do it from the command line. Which student had the furthest location in their trace route? Why do you think that is?

---

## e. TCP and IP
_IP is the system we've just seen, that works with routers to ensure packets of data are split into pieces, sent to the correct destination, and pieced back together. TCP ensures data is properly marked when it is split into pieces, so if one packet does not arrive, the sender is notified and can resend._

### How to Launch the Lesson:
Using the same tool as above have students use the same web tool to count how many locations they went to in their trace route. Did number of places correspond with distance from the previous time using this tool? Why or why not would this make sense? Which website had the least number of hops? Which had the most?

#### Activity: Connections
Give students all a notecard on which is written a different component of an internet connection. Some of them will be packets of data; see if the packets can get to their destination by having students place themselves in the correct order.

---

## f. HTTP
_Hypertext Transfer Protocol, or HTTP, is what web browsers use to speak to web servers. The server receives the request and either successfully executes the action (by rendering a page or submitting a form, for example) or returns an error code; these are called HTTP status codes._

### How to Launch the Lesson:
Find examples of different types of requests. Load the pages with Developer Tools and display the requests to the students.

#### Demo: Status Codes
Find examples of the different status codes on the web (most commonly a 404 or 403), and show them to your students using Chrome's Developer Tools or the like.

---

## g. Trust Models and Open Source
_Every open source piece of software is held to an "open standard" that the software will work in the way intended and not do anything malicious. This involves a significant amount of trust on our end, that whenever we compile a program or visit a website, the pieces of software we use are not injecting malicious code into our computers._

### How to Launch the Lesson:
In small groups, have students research a downloadable software or song. Let them read through the terms and conditions. What sort of things do we agree to that one would be surprised to see? Are we more trusting of certain things than others? What is this trust based on?

---

## h. Cybersecurity
_The Internet is a wonderful resource, but can also occasionally make us vulnerable if we are not following good practices. While we can limit vulnerability to attacks there are many security threats we cannot control and may not even be aware of._

### How to Launch the Lesson:
Students tend to identify with stories they've heard; try to find a cyberattack that has been in the news recently and talk about it! You can probably find a video and show that as well

#### Demo: Insecurity
Find an insecure website (non-https) desiring input of a password or credit card number to show your students how easy it is to spoof something that looks secure.

#### Demo: Permission Levels
If you can display webpages on your localhost to students, you can demonstrate different permission levels on a simple page, talking about why it is beneficial to keep some pages private and only the necessary ones public.

---

## i. HTML
_HTML, or HyperText Markup Language, forms the backbone of web pages. It is used to make any web page you see by formatting all text and images. Students will learn how to create basic web pages using the language._

### How to Launch the Lesson:
Discuss the differences between a mark up language and programming languages. Why do we need two separate languages to do different things? Maybe have students play around with [Khan Academy's HTML module](https://www.khanacademy.org/computing/computer-programming/html-css/intro-to-html/p/html-basics).

#### Demo: Developer Tools
Take a look at an existing website using Chrome's Developer Tools and have your students figure out what the individual tags do.

---

## j. CSS
_CSS, or Cascading Style Sheets, is used to style web pages. It is capable of manipulating colors, positioning, size, alignment, fonts, borders, background shading, and others._

### How to Launch the Lesson:
Have students discuss things that they were unable to do in HTML. Which of those things fall into a styling vs. programming language. How can CSS help? Maybe integrating aspects of [Khan Academy's module on CSS](https://www.khanacademy.org/computing/computer-programming/html-css/intro-to-css/p/css-basics).

#### Demo: Webpage 2.0
Similar to the HTML demonstration, you can create a simple webpage, this time including a CSS sheet to stylize.   

#### Activity: Creativity
Create a simple activity that allows students to be creative with their styling; they can make a basic webpage and choose colors, fonts, shading, etc. 