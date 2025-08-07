Netdata
========================
I was curious about how my hardware is doing. So I searched for a resource monitor. 

I came across Netdata. Reading about how lightweight and that it is easy to use.

To be  fair, the installation was easy.

```
    wget -O /tmp/netdata-kickstart.sh https://get.netdata.cloud/kickstart.sh && sh /tmp/netdata-kickstart.sh
```

I decided to make a cloud account, not knowing that I could access my data from the cloud. So that is cool.

Unfortunately, the configuration was not easy. I might have blocked it in the firewall and thought it was the apps fault not mine.

I don't really like it, to be honest. The dashboard is bloated with unnecessary data, so I need to reconfigure. The cloud option, while secure, eats resources.

Also it opens port 19999, which I don't want to think about that. Therefore I disabled it and I am going to use it from time to time and check if something is going awry.

Nevertheless this showed me I have a problem with my CPU running 100% when opening Jellyfin, so that counts as a plus. :)

This is my configuration file. 
