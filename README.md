# Ad-blocking-guide
A detailed guide for different ad blockers and methods

I made this guide to help people choose their ad blocker and to let people know about different ways of ad blocking.

**Why should you block ads and trackers?**
Digital advertising is an annoyance and a privacy threat. Websites are bloated with ads that make browsing annoying and trackers that mine your data. Then your data will be sold to advertising companies to show more personalized ads.  Preventing unnecessary connections to ads and trackers can save your battery and improve performance. BLocking ads can also protect you from malware, as it's often distributed through malicous ads. 

**But i want to support my favorite sites/creators**
This is a common argument, and it makes completely sense. But remember, digital advertising is harmful. You should support them with other ways, such as donating.

**So how do i start blocking ads**
First, there are multiple ways to block ads. They are roughly categorized them like this:
1. Browser integration
2. DNS filtering
3. Recursive Local VPN
4. Hosts file manipulation
5. External devices

1. The first one is the easiest to implement, but may not be available for all devices, and it includes browser only. You can install https://ublockorigin.com/. It's by far the most complete ad-blocking extension, and is available for most browsers. Only mobile browser compatitable with uBlockOrigin is **Firefox** It supports **cosmetic blocking**. This is useful as it gets rid of elements that can't be blocked by blocking domains.
There are also browsers where ad-blocking is integrated by default. These include Brave, Bromite, Firefox, Opera etc. However, it's always recommended to use uBlock Origin instead of the one provided by the Browser.

2. This one sounds hard, but it's actually quite simple and easy to set up. It works for multiple browsers and platforms including Firefox, Chrome, Windows, Android, iOS and others. You basically find a DNS provider that blocks ads and switch your browser/OS to use that provider. NextDNS is a great provider as it allows you to customize your setup, see logs etc. I suggest looking at https://privacytools.io/providers/dns/ for recommended providers. There are also multiple DNS protocols, mainly plain text, DNS over TLS and DNS over HTTPS. The latter ones are strongly recommended, as it protects your DNS queries from spying and manipulation.
It's always better to use system wide DNS if possible, i suggest looking up a client or a setting to enable it.


3. This one is mainly aimed at mobile users. There are multiple ad blocking apps for Android and iOS that can block ads by using a local VPN. The keyword is local, it's not actually connecting to any remote servers. Here's my recommendations:

Android:
•PersonalDNSfilter
•Blokada
•Adaway

iOS
•Blokada
•NextDNS

4. This one is mostly recommended for PC. You can modify your hosts file to block ads and trackers, but is not generally recommended as it's easy to mess up and hard to keep it updated. You basically find a hosts file that blocks ads There are apps that can do it automatically, such as https://winhelp2002.mvps.org/hosts.txt. This is also possible for Android, but it requires **root access**. A popular app that can block ads using the hosts file is Adaway (in root mode).

5. There are external devices that can block ads and trackers in your whole network, mainly PiHole. Also a big advantage is that this can block ads on other smart devices like your TV. It requires hardware that you keep connected all the time, like Raspberry PI or your PC with Docker. This might not be the best solution for beginners, but i suggest giving it a try.

**Youtube and Facebook ads aren't blocked**
A common problem with mobile is that ads on some apps aren't blocked. This can happen for a these reasons.
1. The ads are from the same domain the content comes from
2. The app bypasses the ad blocker

If the ads come from the same domain the content comes from, it's not possible to block them with domain based blockers. 
