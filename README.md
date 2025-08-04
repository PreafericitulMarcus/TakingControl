# Taking Control
Watching PewDiePie's [video](https://youtu.be/u_Lxkt50xOg?si=SDcBdVsH5MwVnAHd) inspired me to take the steps in order to take control of my digital footprint.

Here is what I did:

## What I chose as replacements

[Heliboard](HeliBoard) &larr; keyboard<br> 
[Signal](https://signal.org/#signal) &larr; messaging app<br>
[QOwnNotes](https://www.qownnotes.org/) &larr; note taking app<br>
[NewPiepe](https://newpipe.net/) &larr; YouTube android client<br>
[Bitwarden](https://bitwarden.com/) &larr; passward manager and 2FA<br>
[Firefox](https://www.firefox.com/en-US/) &larr; main browser<br>


## Self Hosting on local server
Main purpose of the server is for learning experience. 

---
About the server:

 &emsp; On an old desktop I installed Ubuntu Server and set on a journey of learning about self hosting.
 
 

---
Content on the server:

      - [Jellyfin](https://jellyfin.org/) ( currently in development )
      - [SearXNG](https://github.com/searxng/searxng)
      - [NextCloud](https://nextcloud.com/)

Connecting locally for these is easy, but I want to connect remotely and give access to some services to family and friends.

I found there are 3 main options to access these features remotely:

    - [Tailscale](https://tailscale.com/) ( which is easy but not suitable for sharing )
    - Port Forwarding ( I found that opening ports to the public leads to a lot of maintenance )
    - Domain + [Cloudflare](https://www.cloudflare.com/)

I went with Domain + Cloudflare

I also heard about "reverse proxy", which I thought sounded cool and wanted to try implementing one for myself. For that i used Nginx.

You can find about how I configured each service in their respective folders above. But I want to mention that I don't know what I am doing. I am just following YouTube tutorials and ChatGPT. Nevertheless I will learn as I go about setting everything up.
