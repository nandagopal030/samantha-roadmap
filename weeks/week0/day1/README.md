october : 04-10-2026 Place : Home Time : 19:46
https://app.mysamantha.ai/notes/share/618d4d66-df9c-48b0-8ef3-69749c625a53
The plan for week-0 day-1

Week 0: How Software Works (Web, HTML, CSS, JavaScript, First API)
Goal: Build the mental model of how the web works and ship a first live page with real data. For trainees with no web background.
Day 1 (Mon): How the Web Works + Setup
Learn: what happens when a URL is typed (DNS, server, HTTP request, response, render), client vs server, what frontend, backend, database and API mean. Terminal basics (cd, ls, mkdir), files and folders, relative vs absolute paths, VS Code, Live Server, Git + GitHub, browser DevTools (Elements, Console, Network).
Tasks:
Install VS Code, Git, Node.js and an AI coding tool (Claude Code, Codex or OpenCode). Set up ChatGPT or Claude as a tutor for the mornings. Create a GitHub account.
Open any real website, list every request in the Network tab and label each one (HTML, CSS, JS, image, API call).
Draw the URL-to-page flow on paper or in Excalidraw.
Set up a project folder with index.html, styles/ and images/.
Open the page through Live Server and through file:// and note the difference.
Create a repo, make a first commit and push it.
Acceptance Criteria:
Can explain the URL-to-page flow out loud in 2 minutes.
First repo is on GitHub with at least one commit.
No broken asset paths.


* what happens when you type a name or an URL in the website and DNS Explanation
https://www.geeksforgeeks.org/computer-networks/domain-name-system-dns-in-application-layer/
      when i type a word in the browser ex 'bananas' it usually consider it as a search query , when i type a  url 'google.com'in a web browser it will search this URL in the DNS(Domain Name System)
                      USER
                 │
                 │ types URL/search
                 ▼
          ┌──────────────┐
          │   BROWSER    │
          └──────┬───────┘
                 │
          URL or search?
            /          \
          URL          Search
           │              │
           ▼              ▼
          DNS       Search Engine
           │              │
           ▼              ▼
       IP address       Search results
           │
           ▼
        TCP/TLS
           │
           ▼
        HTTPS
           │
           ▼
        WEB SERVER
           │
           ▼
       HTTP RESPONSE
           │
           ▼
        BROWSER
           │
           ▼
      HTML/CSS/JS
           │
           ▼
       WEB PAGE

In depth explantaion 
    User -> www.yahoo.com -> if(DNS) cannot find
                                    |   
                                   DNS Resolver will search for it  if (DNS Resolver connot find) 
                                    |
                                    It will send it to the root server (Root server will have the information of all the domain list) and it will give it to the resolver
                                    |
                                    Now resolver with the list checks with the Top Level Domain Server (TLD) has all the important top level domain list .com.in and so on and now it wll give the list to Resolver
                                    | 
                                    With the new list the resolver will send it to Authoritative Name Server
                                    |
                                    It is responsible for knowing everything and then it will send it to the resolver then resolver stores into a cache for rememberence


* What is a server
https://www.geeksforgeeks.org/computer-networks/what-is-server/
     A server is a computer like machine where it runs through a processors,chips,harddrives,Rams where there are many types of server thet serve different purpose
     A webserver - host the web application and handles the HTTPS req and res
     A Emailserver- Primary purpose Email
     A Database Server  - stores the information and so on

october : 5/10/2026 Time : 11:04 place : Home

* What is Http Request and Response
https://www.geeksforgeeks.org/blogs/http-full-form/
 HTTP - Hypertext transfer protocal
 so it's basically a protocal where it has a set of defined rules to establish a connection between the client and the server and make the request through the browsers and gets the response through the servers and then rendering the html, css, js in the browser 
 There are many versions of HTTP and the modern version works as good as the olderversion like managing the cookies and sessions
  user(client) -> WWW.Valeo..com
               |
   Domain Name service
               |
   returns the IP to client
               |
   client sends the IP to the appropriate server through the request with an action (GET/POST) and payload
               |
   server secures a connection through TCp and then responds with an code (200OK) 
               |
   Client's browser renders the response 
               |
   Connection will get close

* How does the browser renders the response
https://stackoverflow.com/questions/7515227/describe-the-page-rendering-process-in-a-browser
This stackover flow has the answer but i cannot understand fully may be after some week will lookk back into it ****

* what is a client server modal
https://www.youtube.com/watch?v=L5BlpPU_muY
https://www.geeksforgeeks.org/system-design/client-server-model/
A client is a requester and the server is the responder
A client can be a machine / program
A server is a program that listen to the clients req
A client- server modal is a centralized web architecture where there is only a requester and the responder
There is an alternative for client server modal which is peer-to-peer modal where A single machine can be requester and the responder - example torrent / video char skype

* what is a frontend, backend , API and Database
A frontend is a User interface which was being made by HTML,CSS and JS languages
https://chatgpt.com/s/t_6ac34f41f62c8191a2d188f370834b22 

* Basic Terminal commands
https://gist.github.com/bradtraversy/cc180de0edee05075a6139e42d5f28ce

* whats relative vs absolute path
An absolute path specifies a complete file location starting from the root directory, whereas a relative path specifies a file location based on your current working directory

* whats vs code 
Its a open source code editor
Developed by microsoft

* whats a live server
A Live Server is a local development tool that creates a small server on your computer and automatically refreshes your web browser whenever you save changes to your code

* Git & github 
Git is a version control where it saves a specific version of our code as we develop in teams
github is a platform for storing all the version and it also provides the user interface

* Browser DevTools (Elements, console, Network)
Elements are the HTML tags 
Console is the js console log and a error visualizing window
Network is the Req and res identifier

* whats node js and npm
node js runs in a run time environment (real time environment) where it helps the javascript to run outside the browser
npm is a node package manager which has a prewritten code functionality within it where users can downloud using npm i and then work on the code

* What happens when i type Github.com on the browser
         client - github.com
               |
            DNS returns ip address
               |
            client connects to the server through http req
               |
            server responds with status code
               |
            connection close

in this Github.com i had inspected in the console and then checked in the network tab i had found the status code Get action and response in the browser and from the server but i too gets confused why does the response for a single get contains many response in chunks does it works in the chunk way to avoid website speed ??

* Flow chart Task 
https://excalidraw.com/#json=M5Jv5-lJq0KDFZBSfLRhS,h-3X_2QXJxYhCE_71kY7Cw
