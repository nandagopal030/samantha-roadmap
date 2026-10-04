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
     A Database Server  - stors the information and so on
