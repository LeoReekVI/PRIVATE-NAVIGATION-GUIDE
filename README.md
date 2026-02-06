# PRIVATE NAVIGATION GUIDE

This guide aims to teach users how to achieve more private and secure browsing by indicating the best programs, extensions, and settings.

## 1. BROWSERS FOCUSED ON PRIVACY AND SECURITY:

We'll start by choosing a browser. Ideally, the user should use three browsers:
- A primary browser for most everyday activities: with enhanced security and privacy settings, but without sacrificing usability.
- A secondary browser: with normal, i.e., less restrictive settings, to be used if a website does not work in the main browser;
- A specific browser for when you need to perform an activity that requires anonymity or greater security.
See the best options currently available for each case:

### 1.1. MAIN BROWSER INDICATION:

It is recommended that your primary browser be based on Firefox, with the addition of the extensions and settings taught in this guide.

**- [Mozilla Firefox](https://www.mozilla.org/pt-BR/firefox/download/thanks/) + [ArkenFox]( https://github.com/arkenfox/user.js):**
Mozilla Firefox stands out from its competitors due to its privacy, security, advanced configuration options, low RAM consumption, open-source code, and its refusal to adopt Chromium (browsers like Google Chrome, Microsoft Edge, Opera¹, Brave, Chromite, Vivaldi, and others are based on Chromium's source code).

ArkenFox, on the other hand, is a project that maintains a configuration file model (user.js) for Firefox, aiming to harden it for maximum privacy and security, reducing tracking and fingerprinting, while attempting to minimize functionality loss or breakage that may occur. Installation instructions will be provided later. Using ArkenFox with other Firefox-based privacy solutions, such as LibreWolf, Mullvad Browser and Tor Browser is counterproductive.

For Android devices, there is no easy way to implement ArkenFox; the Firefox Beta version, which has access to about:config, is recommended.

**- [LibreWolf](https://librewolf.net/installation/windows/):**
Implementing ArkenFox can be difficult for some users. As a ready-made solution, there is LibreWolf, an independent and pre-hardened fork of Firefox, with anti-fingerprint and anti-tracking improvements, without all the telemetry and services of Mozilla (this makes it lighter), without Google's location service, with a firewall that limits the ability of extensions to initiate connections, and with rapid updates whenever a new version of the Firefox source code is released.

It is available for Windows, Linux, and macOS.

For Android devices, I primarily recommend [Ironfox](https://gitlab.com/ironfox-oss/IronFox/-/releases) (a fork of Mull, which has been discontinued) and secondly [Fennec F- Droid](https://f-droid.org/pt_BR/packages/org.mozilla.fennec_fdroid/).

### 1.2. SECONDARY BROWSER INDICATION:

Considering that these stricter privacy options can hinder the functioning of some websites, it is ideal to keep a Chromium-based browser as a secondary browser, with less restrictive settings (no DNS filtering, no adblock, no tracking protection, etc) to open any website that presents problems in the main browser.

**- [Brave](https://brave.com/):**
Brave is a complete, easier alternative with a more modern look, native adblocker, Tor mode (Tor Browser is better for this purpose), which cleans tracking parameters from URLs, with a VPN option, its own private search engine, etc. Furthermore, it's based on Chromium, which gives it greater compatibility with websites, since many developers only test their sites on Google Chrome, which holds the overwhelming majority of the market. Negative points: it collects data for commercial purposes and places ads from its partners (who pay) in place of blocked ads.

Available for Windows, macOS, Linux, Android and iOS.

**- [Chromite](https://github.com/uazo/cromite/)**
Developed from the discontinued Bromite (a fork), it is based on Chromium with additional security packages from GrapheneOS. It features an ad blocker, fingerprinting protection , DNS over HTTPS support, and other privacy and security enhancements, such as a built-in ad blocker and, in the Android version, a user-script manager.

Available for Windows, Linux, and Android.

**- [Ungoogled Chromium](https://ungoogled-software.github.io/ungoogled-chromium-binaries/)**
Due to some glitches in the Cromite project update, I'm now also recommending Ungoogled Chromium.

Available for Windows, Linux, and macOS.


### 1.3. INDICATION OF ANONYMOUS BROWSER:

If anonymity is desired, it is recommended to use the Tor network or a VPN.

**- [Tor Browser](https://www.torproject.org/download/):**
Tor is the official browser of the Tor project, developed from Firefox and hardened against tracking, fingerprinting, and telemetry, specifically for use on the Tor network, i.e., to provide anonymity (it even hides your IP address). Disadvantages: very slow connection; it is easily detected by some websites that block it; the Tor network is targeted by hackers, governments, and organizations that try to monitor the data transmitted through it, which is done through the exit node that may have been maliciously created or be under control, because the servers are run by volunteers and there is a lack of transparency. However, since Tor changes the nodes used every 10 minutes, this may not be a problem. Avoid using personal data on the Tor network, such as email, website passwords, etc.

Available for Windows, Linux, macOS , and Android. However, it works best on the [Tails](https://tails.net/install/index.pt.html) operating system (designed to run from a USB drive and avoid surveillance and censorship) or on Whonix (runs from a Virtual Machine).

**- [Multivad Browser](https://mullvad.net/en/download/browser/windows/):**
Developed from the Tor Browser, with all its privacy features, however for use with Mullvad VPN (and not the Tor network).

Available for Windows, macOS and Linux.

¹ Opera was bought by a Chinese company involved in scandals, raising doubts about its privacy.

² [PortableApps](https://portableapps.com/apps/) website offers portable versions of major browsers that can be run from a USB drive or external hard drive, allowing you to carry them (with all your settings, extensions, passwords, history, favorites, etc.) and use them on any device without installation, leaving fewer traces on your computer.

³ Check out detailed browser comparisons at [privacytests.org](https://privacytests.org/) and [avoidthehack.com](https://browsers.avoidthehack.com/).

## 2. BASIC PRIVACY AND SECURITY SETTINGS IN FIREFOX:

Access the Firefox (or LibreWolf) settings page and configure it as follows:

1- GENERAL:

1.1- In “Language” **consider** selecting “English (US)” so that websites do not identify your language;

1.2- In "Tabs", check "Enable container tabs";

1.3- In "DRM Content," uncheck "Play DRM-controlled content";

1.4- In "Browsing", uncheck "Recommend extensions while you browse";

1.5- In "Navigation", uncheck "Recommend resources while you browse";

2- START:

2.1- In “Home” and “New tabs” select “Blank page”;

2.2- Uncheck "Sponsored Shortcuts";

2.3- Uncheck "Recent activity";

3- RESEARCH:

3.1- In “Default search engine”, select one of those suggested in topic 3 (such as DuckDuckGo);

3.2- In "Search suggestions," uncheck "Show search suggestions";

4- PRIVACY AND SECURITY:

4.1- In “Enhanced tracking protection”, select “Strict”;

4.2- Check the box "Tell websites not to sell or share my data";

4.3- **Consider** checking "Delete cookies and site data when Firefox is closed";

4.4- **Consider** unchecking "Ask if you want to save passwords" (saving passwords in browsers is not recommended; use dedicated applications/extensions like Bitwarden);

4.4- Click on Permissions > Notifications > Settings and check: Block new permission requests to display notifications;

4.5- Check "Block opening of windows or tabs";

4.6- In "Data collection and use by Firefox", uncheck all options;

4.7- In "Website advertising preferences," uncheck all options;

4.8- In "Security," uncheck "Block dangerous or misleading content" (these options are for checking if the URL is malicious in Google's databases, which generated some tracking until 2011. There have been improvements since then to prevent this, but paranoid users still recommend disabling it);

4.9- In "HTTPS-only mode", select "Enable HTTPS-only mode in all windows"; DoH encrypted DNS provider addresses listed in topic 4 (such as https://dns.adguard-dns.com/dns-query);

5- Customize the browser to display the Search Bar separately from the Address Bar (right-click on an empty part of the Toolbar > customize toolbar > select the Search bar and drag it to the desired position and drop it onto the Toolbar).

6- Install and configure uBlock Origin (taught in topic 5.4).

## 3. PRIVATE SEARCH ENGINES:

Search engines like Google, Bing, and others collect personally identifiable information (PII), IP addresses, location, search history, clicked links, and other data to create a user preference profile for targeted advertising purposes (remember that Google is the world's largest advertising company). The problem is the lack of transparency about what these companies do with the data, whether they share it or sell it to other companies, etc. To make matters worse, they have used their power to lobby for changes in national legislation, further permitting data collection and their lucrative advertising activities. As an alternative, private search engines have emerged, which do not collect data.

To add a search engine in Firefox, do the following: right-click on the Toolbar (in the empty spaces next to the URL field) > click on “Customize Toolbar” > click and drag the “Search” item to the Toolbar and release > access the website of the chosen search engine and click on the “+” that will appear in the search bar > then click on “Add search engine…”.

The search engines below have at least the following characteristics: they do not record or share IP addresses, they do not collect personally identifiable information (PII), they do not use tracking technology, they are free, they do not require registration/login, they are not in alpha or beta development stage, they have Javascript support disabled, and they support Onion Services (Tor) and HSTS.

| Search Engine | Country | Search indexer | DNSSEC | Cryptographic search | Collected aggregate usage metrics | Open source | Anonymous viewing function |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [Brave Search](https://search.brave.com/)[^1] | USA[^4] | Own | Yes | No | Operating system and browser | Yes | No |
| [Startpage](https://www.startpage.com/)[^2] | Netherlands | Google and Bing | Yes | Yes | OS, browser, and language | No | Yes |
| [DuckDuckGo](https://duckduckgo.com/)[^3] | USA[^4] | Bing | No | No | Records research for the product improvement | Partial | No |

[^1]: In Brave Search, it is recommended to disable "anonymous usage metrics" in the settings and always use it without logging in.
[^2]: The Startpage was acquired by the marketing company System1, which alarmed the community regarding the maintenance of privacy standards, but the company stated that it does not possess all rights or autonomy related to user privacy and maintained the standards, calming the public.
[^3]: There is a version of the [DuckDuckGo Lite search engine](https://lite.duckduckgo.com/lite/) that displays results incredibly faster. In tests, Google took 7.56 seconds, DuckDuckGo 2.4 seconds, and DuckDuckGo Lite 0.264 seconds. This is because, while a Google or DuckDuckGo page is about 2 MB, a DuckDuckGo Lite page is only 33 KB. There is also a [DuckDuckGo HTML (or No JavaScript) version](https://html.duckduckgo.com/html/) that is not very different from the Lite version.
[^4]: See the list of countries not recommended in section 7.
[^5]: Honorable Mentions: [MetaGer](https://metager.org/), [Mojeek](https://www.mojeek.com/), [SearXNG](https://docs.searxng.org/), and [Mullvad Leta](https://leta.mullvad.net/).
[^6]: Check out a more detailed comparison of search engines on the [searchengine.party](https://searchengine.party/).

## 4. Encrypted DNS resolvers:

When a user tries to access a website, the browser consults a DNS (Domain Name System) resolver to find out which IP address corresponds to that URL. This is because the IP address identifies the website to the computer and allows access to it. In other words, DNS is a server that functions like a phone book where domains (URLs) and their corresponding IP addresses are listed.

The problem is that these queries can eventually be eavesdropped on (by internet providers, governments, or third parties) and, in more serious cases, can be intercepted and redirected to malicious websites. Therefore, some DNS resolvers use encryption to provide privacy to queries and prevent this from happening.

Today, one of the best encrypted DNS protocols is DoH/3 (DNS over HTTPS version 3), indistinguishable from "normal" HTTPS traffic on port 443 and more difficult to block. However, some metadata, such as user agent (Operating System and Browser), is also sent to the DNS server via DoH .

In 2019, there was some opposition when Firefox pioneered the adoption of DoH , as some experts pointed out weaknesses in this protocol and argued for the superiority of DoT (DNS over TLS)³. Subsequently, the DoH protocol matured, gaining native support in major browsers and operating systems, while DoT did not. Therefore, we will focus on the DoH standard, and more in-depth discussions will not be made here.

The best DNS resolvers offer some filtering option, which blocks malicious domains, trackers, and ads, which is good, but considering that some companies collect data for filtering metrics and new threat detection, in these cases, perhaps the unfiltered version provides greater privacy.

Consider whether it's advantageous for you to define a DNS resolver without filtering in the operating system and one with filtering in your primary browser. This way, if a website has a problem due to the filtering, you can use the secondary browser (which will be using the DNS resolver defined in the OS without filtering). Depending on the programs you use to access the internet, it may be advantageous to have a DNS server with filtering defined in the OS. Therefore, I recommend using Quad9 DNS in your primary browser and AdGuard DNS in Windows (in the latter, choosing between the "with" and "without" filtering options according to your needs).

To set up a DoH DNS resolver in Firefox, go to Menu > Settings > Privacy & Security > Enable DNS over HTTPS using: > select Maximum Protection > click Choose provider: > and paste one of the DoH addresses from the list below.

The DNS resolvers below have, at a minimum, the following characteristics: public, supports DoH (DNS over HTTPS) and DoT (DNS over TLS) encryption protocols, DNSSEC validation, QNAME Minimization, ECS disabled or anonymized, do not store personally identifiable information (PII), and provide some type of filtering against malicious domains.

| DNS resolver | Headquarters | Servers | DoH Version | Data Registration / Privacy Policy | ECS | Type | Filters against |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [Quad9](https://quad9.net/pt/service/service-addresses-and-features/) | Switzerland | Anycast / owned and rented | 1 | Threat response data, remixed and shared for security research purposes. | Optional | Non-profit | Malware |
| [AdGuard](https://adguard-dns.io/pt_br/public-dns.html)[^7] | Cyprus | Anycast rented | 3 | Anonymized performance metrics (number of requests per server and processing speed) and domains requested over 24 hours to identify new trackers and threats. | Anonymized | Commercial with open source code | Malware, ads and pornography |
| [Mullvad](https://mullvad.net/pt/help/dns-over-https-and-dns-over-tls) | Sweden | Own (Germany, Singapore, USA, United Kingdom) and Sweden) | 1 | It does not store any data. | No | Commercial | Malware, ads, tracking, pornography, gambling and social networks |
| [Control D](https://controld.com/free-dns) | Canada | Anycast / own | 3 | Data from customized Premium resolvers. | No | Commercial | Malware, ads, trackers, social networks, pornography, drugs etc |
| [NextDNS](https://my.nextdns.io/)[^8] | USA | Anycast / own | 1 | Data relating to certain functionalities, which can be disabled by the user. | No | Commercial | Several filter options customizable |
| [Cloudflare](https://developers.cloudflare.com/1.1.1.1/setup/) | USA | Anycast / own | 3 | Data from consultation with resolver 1.1.1.1, "the majority" for up to 25 hours. | No | Commercial | Malware and pornography |

[^7]: Adguard supports all other security protocols.
[^8]: NextDNS requires registration to use; the free option limits the filtering feature to 300,000 queries per month, after which the filtering is lost, but encryption remains.
[^9]: Read more at [PowerDNS](https://blog.powerdns.com/2019/09/25/centralised-doh-is-bad-for-privacy-in-2019-and-beyond) and [zdnet](https://www.zdnet.com/article/dns-over-https-causes-more-problems-than-it-solves-experts-say/).
[^10]: Check out comparisons of secure DNS resolvers on the websites [privacyguides.org](https://www.privacyguides.org/en/dns/#recommended-providers), [avoidthehack.com](https://avoidthehack.com/best-dns-privacy), and [privacidade.digital](https://www.privacidade.digital/provedores/dns/).

## 4.1. LIST OF ENCRYPTED DNS SERVER ADDRESSES AND IPs:

### Quad 9 with malware filtering and without ECS:
DoH: https://dns.quad9.net/dns-query

Primary IPv4: 9.9.9.9

Secondary IPv4: 149.112.112.112

Primary IPv6: 2620:fe::fe

Secondary IPv6: 2620:fe::9

### AdGuard DNS without filtering:
DoH: https://unfiltered.adguard-dns.com/dns-query

Primary IPv4: 94.140.14.140

Secondary IPv4: 94.140.14.141

Primary IPv6: 2a10:50c0::1:ff

Secondary IPv6: 2a10:50c0::2:ff

### AdGuard DNS with ad and tracker filtering:
DoH: https://dns.adguard-dns.com/dns-query

Primary IPv4: 94.140.14.14

Secondary IPv4: 94.140.15.15

Primary IPv6: 2a10:50c0::ad1:ff

Secondary IPv6: 2a10:50c0::ad2:ff

### AdGuard DNS with ad, tracker, and pornography filtering:
DoH: https://family.adguard-dns.com/dns-query

Primary IPv4: 94.140.14.15

Secondary IPv4: 94.140.15.16

Primary IPv6: 2a10:50c0::bad1:ff

Secondary IPv6: 2a10:50c0::bad2:ff

### Mullvad DNS with filtering for malware, ads, and trackers:
DoH: https://base.dns.mullvad.net/dns-query

IPv4: 194.242.2.4

IPv6: 2a07:e340::4

### Control D without filtering:
DoH: https://freedns.controld.com/p0

Primary IPv4: 76.76.2.0

Secondary IPv4: 2606:1a40::

Primary IPv6: 76.76.10.0

Secondary IPv6: 2606:1a40:1::

### Control D with filtering for malware, ads, and trackers:
DoH: https://freedns.controld.com/p2

Primary IPv4: 76.76.2.2

Secondary IPv4: 2606:1a40::2

Primary IPv6: 76.76.10.2

Secondary IPv6: 2606:1a40:1::2

### Control D with filtering for malware, ads, trackers, pornography, and drugs:
DoH: https://freedns.controld.com/family

Primary IPv4: 76.76.2.4

Secondary IPv4: 2606:1a40::4

Primary IPv6: 76.76.10.4

Secondary IPv6: 2606:1a40:1::4

### NextDNS (configure filtering options on the website):
DoH: https://firefox.dns.nextdns.io/

**Cloudflare DNS without filtering:**
DoH: https://cloudflare-dns.com/dns-query

DoH (Firefox): https://mozilla.cloudflare-dns.com/dns-query

Primary IPv4: 1.1.1.1

Secondary IPv4: 1.0.0.1

Primary IPv6: 2606:4700:4700::1111

Secondary IPv6: 2606:4700:4700::1001

### Cloudflare DNS with malware filtering:
DoH: https://security.cloudflare-dns.com/dns-query

Primary IPv4: 1.1.1.2

Secondary IPv4: 1.0.0.2

Primary IPv6: 2606:4700:4700::1112

Secondary IPv6: 2606:4700:4700::1002

### Cloudflare DNS with malware and pornography filtering:
DoH: https://family.cloudflare-dns.com/dns-query

Primary IPv4: 1.1.1.3

Secondary IPv4: 1.0.0.3

Primary IPv6: 2606:4700:4700::1113

Secondary IPv6: 2606:4700:4700::1003

## 4.2. HOW TO CONFIGURE DoH SERVER ON WINDOWS 11:

1. Press Win + I (to access Settings > Network & Internet);

2- If using a wireless connection, click on Wi-Fi;

3- Click on “Hardware Properties”;

4- In “DNS Server Assignment” click on “Edit”;

5- In “Edit DNS settings” select “Manual”;

6- Disable IPv4 (IPv6 is now the internet standard and offers security advantages);

7- Enable IPv6;

8- In “Preferred DNS” enter the first IPv6 address corresponding to the desired server (see the list above);

9- In “DNS over HTTPS” select “Enabled (manual template)”;

10- In “DNS over HTTPS model” enter the DoH address corresponding to the desired server (see the list above);

11- In “Fallback to encrypted text” leave “Disabled”;

12- In “Alternative DNS” enter the second IPv6 address corresponding to the desired server (see the list above);

13- Configure the rest the same as in steps 10 to 12;

14- If using a wired connection, click on Ethernet;

15- In “DNS Server Assignment” click on “Edit”;

16- Repeat the same configuration as in steps 4 to 13.

## 5. EXTENSIONS

Extensions add new functions to your browser and can improve your privacy and security.
However, only use extensions from trusted sources and try not to use too many, as this can increase the attack surface and fingerprint.

### 5.1. ESSENTIAL EXTENSION:

**- [uBlock Origin](https://addons.mozilla.org/pt-BR/firefox/addon/ublock-origin/):** the best adblocker currently available, stands out for its superior blocking rules (both in syntax and repository), low RAM consumption, and diverse features. Check the recommended settings in section 5.2.

An ad blocker , as the name suggests, is used to block advertisements, but it does much more than that; it blocks domains that are sources of malware, scams, phishing, tracking, and allows you to add specific blocking filters, such as against pornography, social networks, gambling, piracy, fake news, paywall, etc.

Examples of things that are blocked: YouTube ads; cookie notices on websites; pop-ups that disrupt browsing; embarrassing ads; misleading buttons that appear on download sites that lead the user to download unwanted things; notices on websites that ask for payment to read more news.

As a result, it promotes greater security, privacy, browsing speed (due to the elimination of the need to download blocked elements), and improves the appearance of websites (due to blocked ads).

Trackers on websites can obtain information about you, such as: IP address, location, click-through rate of other ads, websites visited, screen resolution, device type, operating system, browser data, language, browsing habits, time zone, clipboard information, information filled in on forms, etc. Using a good ad blocker minimizes this.

Internet browsing is the main gateway that allows criminals to access devices, which is why the security provided by an ad blocker is so significant. Its use is as essential as that of an antivirus program; in fact, even the [CIA](https://www.vice.com/en/article/the-nsa-and-cia-use-ad-blockers-because-online-advertising-is-so-dangerous/) and [FBI](https://en.as.com/latest_news/the-reason-why-the-fbi-says-you-should-use-an-ad-blocker-n/) recommend it.

### 5.2. RECOMMENDED EXTENSIONS:

**- [NoScript](https://addons.mozilla.org/en-US/firefox/addon/noscript/):** Blocks scripts (Java, Flash, Silverlight, and others) and allows you to set permissions per site. uBlock Origin may perform the primary function of blocking JavaScript, but NoScript offers protection against XSS and Clickjacking attacks, prevention of malicious META redirects, and XSLT blocking. Using JavaScript blocking can lead to a poor browsing experience, so try checking “Globally allowed JavaScript”.

**- [Firefox Multi-Account Containers](https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/):** Allows you to open separate websites in containers for specific categories (Shopping, Personal, Work, Social Networks, etc) according to your configuration, where the containers do not share cookies and data with each other, providing greater security and privacy and allowing you to keep parts of your online life separate. Implementation of Total Cookie Protection (dFPI) in Firefox has somewhat diminished its usefulness in terms of security, as third-party cookies are already partitioned; however, it provides additional benefits such as an extra layer of isolation, logging into multiple accounts on the same website using different containers, and advanced VPN and proxy settings (using it with Mozilla VPN allows the user to configure specific containers for a specific VPN server). To open a website in a specific container, simply click the button that appears on the right side of the address bar and select the desired container.

**- [Temporary Containers](https://addons.mozilla.org/en-US/firefox/addon/temporary-containers/):** Allows you to open websites and links in disposable containers that isolate website data (cookies, storage, and more) and automatically delete this data when the container is closed, increasing your privacy and security. Unlike the previous method, cookies and data are not separated by category, but completely isolated for that specific website. API compatible with dFPI. No longer maintained.

**- [ViolentMonkey](https://violentmonkey.github.io/):** An open-source userscript manager. It provides userscript support for browsers, allowing you to customize how a web page is displayed or behaves, as well as add useful functions to the browser, through small snippets of JavaScript code that can be written by the user or downloaded from internet repositories. See below for suggestions of useful scripts.
Warning: User-generated scripts generate a large amount of fingerprinting and can present serious privacy and security risks, as they increase the attack surface and rely heavily on trust in their creators.

**- [Skip Redirect](https://addons.mozilla.org/en-US/firefox/addon/skip-redirect/):** Some websites use intermediate pages before redirecting to the final page. This add-on attempts to extract the final URL from the intermediate URL and redirect there immediately. Unfortunately, it doesn't always work.

**- [Privacy-Oriented Origin Policy (POOP)](https://addons.mozilla.org/en-US/firefox/addon/privacy-oriented-origin-policy/):** Handles Cross-Origin requests. Resource Sharing (CORS). Recommended configuration: set 'Global mode' to 'aggressive', enable the options 'Exclude root domain matches' and 'Spoof cross-origin referer'. You can also add the following to the exclusions area:

```
www.youtube.com *.googlevideo.com
www.youtube-nocookie.com *.googlevideo.com
*.dailymotion.com *.dmcdn.net
```

**- [Bitwarden](https://addons.mozilla.org/en-US/firefox/addon/bitwarden-password-manager/):** The highest-rated open-source password manager according to experts. Using the browser's password manager is not recommended. The downside is its moderate RAM consumption.

**- AdGuard:** A well-known ad blocker, however, considering that uBlock Origin uses its own filter lists, or we can use them through the AdGuard DNS resolver, making its use redundant.

**- LocalCDN:** Similar to Decentraleyes, but supports many more frameworks (108 versus 15) and has more frequent updates. While using local CDNs works with the included scripts, it's not a comprehensive solution and doesn't work with most third-party connections, and it can increase fingerprinting. This extension is less useful after the implementation of Total Cookie Protection in Firefox. If you want to use it yourself, see the setup guide in section 5.7.

**- CanvasBlocker:** Anti-fingerprinting extension; its use is redundant after the implementation of the RFP (Resist FingerPrinting) and FPP (FingerPrinting Protection) in Firefox. It is only useful if you disable RFP or if you enable WebGL. If you want to use it yourself, see the configuration guide in section 5.9.

Check out relevant information about extensions on the websites [privacyguides.org](https://www.privacyguides.org/articles/2021/12/01/firefox-privacy-2021-update/), [12bytes](https://codeberg.org/12bytes/firefox-config-guide), and the [ArkenFox Wiki](https://github.com/arkenfox/user.js/wiki/4.1-Extensions).

### 5.3. EXTENSIONS NOT RECOMMENDED:

**- Adblock Plus:** a closed-source program maintained by a private company that has an "acceptable ads" program, where companies can pay to avoid having their ads blocked. It has less efficient blocking and higher RAM consumption compared to uBlock Origin.

**- ClearURLs:** redundant since uBlock Origin added the “removeparam” function; simply add the Dandelion filter. ClearURLs for uBo (topic 5.4).

**- CSS Exfil Protection:** Virtually zero threat, and if the platform's CSS were compromised, you would have much bigger problems to worry about.

**- Dark Reader:** causes performance issues and increases fingerprinting.

**- Decentralized Eyes:** While using local CDNs works with the included scripts, it's not a comprehensive solution and doesn't work with most third-party connections, plus it can increase fingerprinting. This extension is very outdated and less useful after the implementation of Total Cookie Protection in Firefox. LocalCDN is more up-to-date and supports many more frameworks.

**- Disconnect:** it's better to use uBlock. Origin, along with Firefox's Total Cookie Protection.

**- Don't Track Me Google:** unnecessary if you use uBlock. Origin, along with Firefox's Total Cookie Protection, recommends using a private browser, as explained in topic 2. It also exists as a script for ViolentMonkey and similar programs, as explained in topic 5.5.

**- Anti-fingerprinting extensions (such as CanvasBlocker):** redundant after RFP implementation (Resist Finger Printing) and FPP (Fingerprint Printing Protection) in Firefox. It is only useful if you disable RFP in Firefox or if you enable WebGL.

**- Spell checking extensions (like Grammarly or LanguageTool):** send all your typing data to a remote server, a privacy nightmare.

**- Extensions for deleting cookies:** browsers already offer the option to delete cookies when closing, and with Total Cookie Protection in Firefox, this becomes less necessary.

**- Ghostery:** a closed source program maintained by a private advertising company.

**- Google Search Link Fix:** unnecessary if using uBlock Origin, along with Firefox's Total Cookie Protection, can also be used with a private search engine, as explained in topic 2.

**- HTTPS Everywhere:** This is unnecessary since HTTPS-only mode was adopted by browsers and, therefore, has been discontinued.

**- I don't care about cookies:** it was acquired by Gen Digital, a giant that, through acquisitions and mergers, has become the owner of several popular anti-malware and cybersecurity application companies, such as Avira, Avast, AVG, Norton, Symantec, CCleaner, etc. Its programs are known for promoting mass tracking and exhibiting suspicious behavior. Its ad blocker list can still be used safely.

**- Nano Adblocker and Nano Defender:** the project was sold to a company that altered the code to use it as spyware/malware in Chromium-based versions. The Firefox version has another developer and remained secure, however, after this news, users abandoned its use and the project was discontinued.

**- Neat URL and CleanLinks:** redundant with uBlock Since the "removeparam" function was added, simply add the AdGuard URL Tracking Protection filters (native to uBlock Origin) and Dandelion Actually Legitimate URL Shortener Tool (topic 5.4).

**- Other adblock extensions:** using multiple adblock extensions can interfere with each other's functionality. Today, uBlock... Origin is the best option.

**- Privacy Badger and Privacy Possum:** considering that they no longer use heuristics (although heuristics can increase fingerprint), they became unnecessary after the implementation of Total Cookie Protection in Firefox and if you use uBlock Origin. Besides, it's outdated.

**- Smart Referer:** Omits the Referer header from HTTP(S) requests, unless the request is to the same domain as the page you are already on. The Referer header This includes the address of the page you were on before navigating to the current page. This can be used for tracking. Best practices in browsers for HTTPS websites have made this extension unnecessary.

**- uMatrix:** has not been updated since 2019.

### 5.4. RECOMMENDED SETTINGS IN UBLOCK ORIGIN:

In Chromium-based browsers such as Edge, Ungoogled Chromium, Cromite, Brave, Vivaldi, DuckDuckGo, and Opera (except Google Chrome), it is possible to install uBlock Origin.

The most effective installation method is as follows:

1. Access [https://github.com/gorhill/uBlock/releases]( https://github.com/gorhill/uBlock/releases);

2. In the first version that appears, click on Assets and download the chromium.zip file;

3. Unzip the downloaded file;

4. Open the browser, go to Menu > Extensions > click on Manage Extensions;

5. Enable the “Developer mode” option;

6. Click on “Load without package” and select the extracted folder.

### 5.5. RECOMMENDED SETTINGS IN UBLOCK ORIGIN:

Within your browser, click the uBlock Origin extension icon. Go to Origin and click on the gears to open the settings and configure them as follows:

SETTINGS:
- Disable prefetching (to prevent any requests from blocked networks) -> ✅
- Disable hyperlink auditing -> ✅
- Prevent WebRCT from leaking your local IP address -> ✅ (option removed from uBlock Origin for desktop browsers since version 1.38)
- Block CSP reports -> ✅
- Reveal canonical names -> ✅
- I am an advanced user -> ✅

ADVANCED:

Click on the gear icon next to the "I am an advanced user" option to enter the advanced settings and configure it as follows:

autoCommentFilterTemplate = {{url}}

autoUpdateDelayAfterLaunch = 10 (update outdated filter lists x seconds after browser initialization)

disableWebAssembly = true

filterAuthorMode = true (enable dynamic filtering)

trustedListPrefixes = -

updateAssetBrowserCache = true (ignore the cache when manually fetching a filter list more than once per hour)

FILTER LISTS:
- Automatically update filter lists -> ✅
- Suspend network activity until all filter lists are loaded -> ✅
- Analyze and apply cosmetic filters -> ✅
- Ignore generic cosmetic filters -> ❌
- Select all desired filters: (consider leaving AdGuard Mobile Ads unchecked if you are on a desktop, Social Widgets if you use social media, and only check the Regional/Language filter corresponding to yours)

Source: [uBlock Origin GitHub](https://github.com/uBlockOrigin/uBlock-issues/wiki/Blocking-mode), by developer [Raymond Hill](https://github.com/gorhill/uBlock/wiki/Advanced-settings#blockingprofiles), [Yokoffing](https://github.com/yokoffing/filterlists?tab=readme-ov-file#advanced-settings), and [Celenity](https://codeberg.org/celenity/ublock-origin-settings).

### 5.6. HARD LOCK SETTINGS IN UBLOCK ORIGIN:

> [!Warning]
> Hard blocking mode greatly increases privacy and security, but it causes frequent website crashes. These crashes can be circumvented, as explained below, but they are an inconvenience to the online browsing experience. Therefore, assess your need for them.

In Settings:
- Disable JavaScript -> ✅

If any website experiences a break, simply open the options panel and click on the </> icon to remove the red "X" over it and refresh the page (F5). This will enable JavaScript on that specific domain.

Copy the three lines below and paste them into the My Rules tab, under Temporary Rules, and then click Confirm:

```
* * 3p block
* * 3p-script block
* * 3p-frame block
```

If any website experiences breakage, simply open the options panel and click on the red squares, leaving them uncolored. The "third-party" square corresponds to the first line above and is the one that most often causes breakages, so unchecking it may correct the problem. The "third-party scripts" and "third-party frames" squares correspond to the second and third lines above, respectively. Unchecking all three temporarily disables hard protection (returns to normal protection mode).

### 5.7. RECOMMENDED FILTER LISTS FOR BLOCKING:

In Filter Lists, at the bottom, click “Import” and, in the box that appears, paste the web address lines corresponding to the filter lists you want to add, then confirm by clicking “Apply changes” at the top.
See below for some recommendations:

```
BASIC ALL-IN-ONE LISTS:

⭐️ AdBlocker Ultimate Filters (compilation of uBlock Origin, Adguard and Easy/Fanboy’s lists):
AdBlocker Ultimate Ad Filter (170k): https://filters.adavoid.org/ultimate-ad-filter.txt
AdBlocker Ultimate Privacy Filter (163k): https://filters.adavoid.org/ultimate-privacy-filter.txt
AdBlocker Ultimate Security Filter (12k): https://filters.adavoid.org/ultimate-security-filter.txt

Fanboy Ultimate List (215k / includes Easy/Fanboy’s Lists = Easylist, Easyprivacy, Fanboy Enhanced Trackers and Fanboy Annoyances (includes Fanboy Social, Fanboy Anti-cookie Warnings and Fanboy Notifications List): https://secure.fanboy.co.nz/r/fanboy-ultimate.txt

AdGuard DNS (107k / includes social media, privacy/spyware, mobile, EasyList and EasyPrivacy): https://raw.githubusercontent.com/AdguardTeam/FiltersRegistry/master/filters/filter_15_DnsFilter/filter.txt

StevenBlack (166k / includes AdAway, Dan Pollock - someonewhocares.org, MVPS hosts, Peter Lowe - yoyo.org, URLHaus, hostVN, FadeMint, KADhosts, Mitchell Krog’s, minecraft, Tiuxo, UnckeckyAds): https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts

MULTIPURPOSE LISTS:

⭐️ HaGeZi's DNS Blocklist Pro Mini (65k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.mini.txt

HaGeZi's Multi DNS Blocklist Pro Full (167k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.txt

HaGeZi's Multi DNS Blocklist Pro++ Mini (89k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.plus.mini.txt

HaGeZi's Multi DNS Blocklist Pro++ Full (288k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/pro.plus.txt

HaGeZi's Multi DNS Blocklist Ultimate Mini (103k / breakage): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/ultimate.mini.txt

HaGeZi's Multi DNS Blocklist Ultimate Full (340k / breakage): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/ultimate.txt

Combined Privacy Block Lists (CPBL) for adblock Mini (98k): https://raw.githubusercontent.com/bongochong/CombinedPrivacyBlockLists/refs/heads/master/MiniLists/cpbl-abp-mini.txt

Combined Privacy Block Lists for adblock (156k): https://raw.githubusercontent.com/bongochong/CombinedPrivacyBlockLists/master/cpbl-abp-list.txt

OISD Blocklist small (44k): https://small.oisd.nl

⭐️ OISD Blocklist big (179k): https://big.oisd.nl/

1Hosts Lite (58k): https://raw.githubusercontent.com/badmojr/1Hosts/master/Lite/adblock.txt

1Hosts Pro (143k / breakage): https://raw.githubusercontent.com/badmojr/1Hosts/master/Pro/adblock.txt

⭐️ Adaway (6,5k): https://adaway.org/hosts.txt

⭐️ Peter Lowe's hosts (3,4k): https://pgl.yoyo.org/adservers/serverlist.php?hostformat=adblockplus&showintro=1&mimetype=plaintext

⭐️ Dan Pollock’s hosts (11,7k): https://someonewhocares.org/hosts/hosts

MVPS hosts (8,7k / outdated): https://winhelp2002.mvps.org/hosts.txt

SNAFU Blocklist (62k): https://raw.githubusercontent.com/RooneyMcNibNug/pihole-stuff/master/SNAFU.txt

GoodbyeAds Filters (278k): https://raw.githubusercontent.com/jerryn70/GoodbyeAds/master/Formats/GoodbyeAds-AdBlock-Filter.txt

hBlock Host (598k): https://hblock.molinero.dev/hosts_adblock.txt

Divested Host (856k): https://divested.dev/hosts-domains-wildcards


ANTI-ADVERTISING LISTS:

Firebog WaLLy3K’s Admiral (>1k): https://v.firebog.net/hosts/Admiral.txt

Firebog WaLLy3K’s Pringent Ads (4k): https://v.firebog.net/hosts/Prigent-Ads.txt

AWAvenue Ads Rule (>1k): https://raw.githubusercontent.com/TG-Twilight/AWAvenue-Ads-Rule/main/AWAvenue-Ads-Rule.txt

Shadow Whisperer Ads (21k): https://raw.githubusercontent.com/ShadowWhisperer/BlockLists/master/Lists/Ads

Disconnect Advertising Filter List (3k / outdated): https://s3.amazonaws.com/lists.disconnect.me/simple_ad.txt

AdGuard CNAME-ads (9,8k): https://raw.githubusercontent.com/AdguardTeam/cname-trackers/master/data/combined_disguised_ads.txt

ANTI-TRACKING LISTS:

Quidsup NoTrack Tracker Blocklist (16k): https://gitlab.com/quidsup/notrack-blocklists/raw/master/notrack-blocklist.txt

FrogEye (33k): https://hostfiles.frogeye.fr/firstparty-trackers-hosts.txt

NoTraking Hosts (420k / outdated): https://raw.githubusercontent.com/notracking/hosts-blocklists/master/adblock/adblock.txt

Energized Exodus Privacy (>1k): https://energized.pro/mirror/exodus-privacy-trackers.txt

Exodus Privacy Blokada version (>1k): https://blokada.org/mirror/v5/exodusprivacy/standard/hosts.txt

Energized DuckDuckGo Tracker Radar (1k): https://energized.pro/mirror/duckduckgo-tracker-blocklists.txt

DuckDuckGo Radar Blokada version (12,6k): https://blokada.org/blocklists/ddgtrackerradar/standard/hosts.txt

Energized Ghostery WhoTracks.me (3k): https://energized.pro/mirror/whotracks-me.txt

AdGuard CNAME-trackers (163k): https://raw.githubusercontent.com/AdguardTeam/cname-trackers/master/data/combined_disguised_trackers.txt

Abine DNT (>1k / outdated): https://raw.githubusercontent.com/HxxxxxS/Blocklists/master/lists/Abine-DNT.txt

Disconnect Tracking Filter List (>1k / outdated): https://s3.amazonaws.com/lists.disconnect.me/simple_tracking.txt

REMOVE TRACKING URL PARAMETERS LISTS:

⭐️ Dandelion Sprout’s Actually Legitimate URL Shortner Tool (2,7k): https://raw.githubusercontent.com/DandelionSprout/adfilt/master/LegitimateURLShortener.txt

AdGuard Tracking URL Parameters (2k): https://raw.githubusercontent.com/AdguardTeam/FiltersRegistry/master/filters/filter_17_TrackParam/filter.txt

Dandelion Sprout’s ClearURLs (>1k / based on ClearURLs extension): https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ClearURLs%20for%20uBo/clear_urls_uboified.txt

PRIVACY LISTS:

⭐️ Yokoffing's Block third-party fonts (>1k / better than the original Fanboy):
https://raw.githubusercontent.com/yokoffing/filterlists/main/block_third_party_fonts.txt

⭐️ Yokoffing's Click2Load (>1k): https://raw.githubusercontent.com/yokoffing/filterlists/main/click2load.txt

Yokoffing's Privacy Essentials (>1k / includes Click2Load / breakage): https://raw.githubusercontent.com/yokoffing/filterlists/main/privacy_essentials.txt

⭐️ Divested Fingerprinting (>1k): https://divested.dev/blocklists/Fingerprinting.ubl

⭐️ DeveloperDan Lightswitch05's AMP (Google's Accelerated Mobile Pages) hosts (16k / for mobiles): https://www.github.developerdan.com/hosts/lists/amp-hosts-extended.txt

Curben Fingerprinting by JS (253k): https://curbengh.github.io/malware-filter/tracking-filter.txt

ANTI-ANNOYANCE LISTS:

Easylist Adblock Warning Removal List (2k / are there any contraindications for use with uBlock Origin): https://easylist-downloads.adblockplus.org/antiadblockfilters.txt?a=1

Nano Defender (2,6k / outdated / are there any contraindications for use with uBlock Origin): https://raw.githubusercontent.com/NanoAdblocker/NanoFilters/master/NanoMirror/NanoDefender.txt

Anti-Circumvention AdBlock Plus (>1k / are there any contraindications for use with uBlock Origin): https://easylist-downloads.adblockplus.org/abp-filters-anti-cv.txt?a=1

Yokoffing's Annoyance List (>1k): https://raw.githubusercontent.com/yokoffing/filterlists/main/annoyance_list.txt

Dandelion Sprout’s Fanboy Notifications (3k / better than the original): https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Other%20domains%20versions/FanboyNotifications-LoadableInUBO.txt

ANTI-MALWARE LISTS:

⭐️ HaGeZi's Most Abused TDLs (>1k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/spam-tlds-ublock.txt

⭐️ Dandelion Sprout’s Anti-Malware List (144k): https://raw.githubusercontent.com/DandelionSprout/adfilt/refs/heads/master/Dandelion%20Sprout's%20Anti-Malware%20List.txt

Dandelion Sprout’s Annoyances List (148k / includes Sprout’s Dandelion anti-malware List and Sprout’s Dandelion Without Logging List): https://raw.githubusercontent.com/DandelionSprout/adfilt/master/AnnoyancesList

⭐️ iam-py-test's The malicious website blocklist (38k): https://raw.githubusercontent.com/iam-py-test/my_filters_001/refs/heads/main/antimalware.txt

iam-py-test's uBlock Combo (153k / includes iam-py-test's The malicious website blocklist, Dandelion Sprout’s Anti-Malware List, Dandelion Sprout’s Legitimate URL Shortner Tool and iam-py-test's anti-typo list): https://raw.githubusercontent.com/iam-py-test/uBlock-combo/refs/heads/main/list.txt

⭐️ FMHY Unsafe Sites Filterlist (>1k): https://raw.githubusercontent.com/fmhy/FMHYFilterlist/main/filterlist.txt

Stalkerware Indicators List (>1k): https://raw.githubusercontent.com/AssoEchap/stalkerware-indicators/master/generated/hosts

BarbBlock (>1k): https://paulgb.github.io/BarbBlock/blacklists/ublock-origin.txt

Quidsup NoTrack Malware Blocklist (>1k): https://gitlab.com/quidsup/notrack-blocklists/raw/master/notrack-malware.txt

Team CYMRU Bogon List (2,8k): https://www.team-cymru.org/Services/Bogons/fullbogons-ipv4.txt

CyberHost Malware and Phishing (12k): https://lists.cyberhost.uk/malware.txt

The Big List of Hacked Malware Web Sites (20k): https://raw.githubusercontent.com/mitchellkrogza/The-Big-List-of-Hacked-Malware-Web-Sites/refs/heads/master/.input_sources/hacked-malware-websites.txt

Shadow Whisperer Malware (45k): https://raw.githubusercontent.com/ShadowWhisperer/BlockLists/refs/heads/master/Lists/Malware

Firebog WaLLy3K’s Pringent Malware (180k): https://v.firebog.net/hosts/Prigent-Malware.txt

Disconnect Malware Filter Domains (1k / outdated): https://raw.githubusercontent.com/deathbybandaid/piholeparser/master/Subscribable-Lists/ParsedBlacklists/Disconnect-Malware-Filter.txt

Disconnect Malvertising Filter List (3k / outdated): https://s3.amazonaws.com/lists.disconnect.me/simple_malvertising.txt

THREATS INTELLIGENCE LISTS:

⭐️ HaGeZi's Threat Intelligence Feeds Mini (78k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/tif.mini.txt

HaGeZi's Threat Intelligence Feeds Medium (337k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/tif.medium.txt

HaGeZi's Threat Intelligence Feeds Full (685k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/tif.txt

Emerging Threats PiHole (3k): https://hosts.tweedge.net/malicious.txt

Threat Fox (65k): https://threatfox.abuse.ch/downloads/hostfile/

ANTI-SCAM LISTS:

⭐️ Scam Blocklist by DurableNapkin (>1k): https://raw.githubusercontent.com/durablenapkin/scamblocklist/master/adguard.txt

Malware Filter Phishing (>1k): https://malware-filter.gitlab.io/malware-filter/phishing-filter-hosts.txt

⭐️ Spam404 (7k): https://raw.githubusercontent.com/Spam404/lists/master/adblock-list.txt

Phishing Army Blocklist (82k): https://phishing.army/download/phishing_army_blocklist.txt

ANTI-COIN MINERS LISTS:

NoCoin AdBlock Plus (>1k): https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt

NoCoin hosts (>1k): https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/hosts.txt

Firebog WaLLy3K’s Pringent Crypto (16k): https://v.firebog.net/hosts/Prigent-Crypto.txt

BYPASS PAYWALLS AND LOGGIN LISTS:

⭐️ Magnolia Bypass Paywalls Clean filters (1k): https://gitflic.ru/project/magnolia1234/bypass-paywalls-clean-filters/blob/raw?file=bpc-paywall-filter.txt

Liam anti-paywall (2k): https://raw.githubusercontent.com/liamengland1/miscfilters/master/antipaywall.txt

Dandelion Sprout’s Without Logging (>1k): https://raw.githubusercontent.com/DandelionSprout/adfilt/master/BrowseWebsitesWithoutLoggingIn.txt

iam-py-test's Anticookie and Sign-up (>1k): https://raw.githubusercontent.com/iam-py-test/my_filters_001/refs/heads/main/anti-cookie%2Bsign%20up.txt

Yokoffing antipaywall filters (>1k): https://raw.githubusercontent.com/yokoffing/filterlists/refs/heads/main/antipaywall_filters_without_element_hiding.txt

OTHER HAGEZI’S LISTS:

HaGeZi's Dynamic DNS (>1k / phishing): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/dyndns.txt

HaGeZi's Badware Hoster DNS Blocklist (2k): https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/hoster.txt

HaGeZi's Encrypted DNS Bypass Blocklist (1,4k / breakage): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/doh.txt

HaGeZi's URL Shorteners Whitelist / Allowlist (5,4k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/whitelist-urlshortener.txt

HaGeZi's Whitelist / Allowlist Referral (>1k): https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/whitelist-referral.txt

OTHER CELENITY’S LISTS:

⭐️ Celenity BadBlock Lite (16k): https://badblock.celenity.dev/abp/badblock_lite.txt

Celenity BadBlock (16k / breakage): https://badblock.celenity.dev/abp/badblock_lite.txt

Celenity BadBlock+ (16k / breakage): https://badblock.celenity.dev/abp/badblock_plus.txt

Celenity’s Whitelist (6k): https://badblock.celenity.dev/abp/whitelist.txt

Celenity’s Block-SVG (>1k): https://badblock.celenity.dev/hardened/block-svg.txt

Celenity’s Unbreak Block-SVG (>1k): https://badblock.celenity.dev/hardened/unbreak-svg.txt

Celenity’s Block-WebGL (>1k): https://badblock.celenity.dev/hardened/block-webgl.txt

Celenity’s Unbreak Block-WebGL (>1k): https://badblock.celenity.dev/hardened/unbreak-webgl.txt

Celenity’s Block-WebGPU (>1k): https://badblock.celenity.dev/hardened/block-webgpu.txt 

Celenity’s Unbreak Block-WebGPU (>1k): https://badblock.celenity.dev/hardened/unbreak-webgpu.txt

Celenity’s Block-WebRCT (>1k): https://badblock.celenity.dev/hardened/block-webrtc.txt

Celenity’s Unbreak Block-WebRTC (>1k): https://badblock.celenity.dev/hardened/unbreak-webrtc.txt

Celenity’s Click-Tracking (>1k): https://badblock.celenity.dev/abp/click-tracking.txt

Celenity’s DoH / stop DNS bypass (>1k): https://badblock.celenity.dev/abp/doh.txt

Celenity’s block websites associated with DRM (>1k): https://badblock.celenity.dev/abp/drm.txt

Celenity’s Block Beacon (>1k): https://gitlab.com/celenityy/Phoenix/-/raw/pages/uBlock/beacon.txt

Celenity’s block crap / toxic domains (>1k): https://badblock.celenity.dev/abp/crap.txt

Celenity’s block find my device (>1k): https://badblock.celenity.dev/abp/find-my.txt

OTHER DANDELION SPROUT’S LISTS:

Dandelion Sprout’s Anti-'Functionality removal' text copying and right-clicking (>1k): https://raw.githubusercontent.com/DandelionSprout/adfilt/master/AntiFunctionalityRemovalList.txt

Dandelion Sprout’s Unusual Ads (>1k): https://raw.githubusercontent.com/DandelionSprout/adfilt/master/AdRemovalListForUnusualAds.txt

Dandelion Sprout’s Suspicious (9k): https://raw.githubusercontent.com/DandelionSprout/adfilt/refs/heads/master/AdGuardHomeDisallowedIPs.txt

Dandelion Sprout’s Extremely Condensed List (>1k): https://raw.githubusercontent.com/DandelionSprout/adfilt/master/ExtremelyCondensedList.txt

OTHER IAM-PY-TEST LISTS:

iam-py-test's Anti-Dynamic DNS (>1k): https://raw.githubusercontent.com/iam-py-test/my_filters_001/refs/heads/main/antidynamicdns.txt

iam-py-test's Anti-"Private analytics" (>1k): https://raw.githubusercontent.com/iam-py-test/my_filters_001/refs/heads/main/anti-privacy-analytics.txt

iam-py-test's Anti-Redirectors (>1k): https://raw.githubusercontent.com/iam-py-test/my_filters_001/refs/heads/main/anti-redirectors.txt

iam-py-test's Clickbait blocklist (>1k): https://raw.githubusercontent.com/iam-py-test/my_filters_001/refs/heads/main/clickbait.txt

iam-py-test's IP Lookup Service Blocklist (>1k): https://raw.githubusercontent.com/iam-py-test/my_filters_001/refs/heads/main/antiiplookup.txt

iam-py-test's Anti-Norton (>1k): https://github.com/iam-py-test/my_filters_001/raw/refs/heads/main/anti-norton.txt

iam-py-test's anti-PUP (>1k): https://raw.githubusercontent.com/iam-py-test/my_filters_001/refs/heads/main/antipup.txt

OTHER ENERGIZED LISTS:

Energized Spark (85k): https://energized.pro/spark/adblock.txt

Energized Blu (188k): https://energized.pro/blu/adblock.txt

Energized Ultimate (510k): https://energized.pro/ultimate/adblock.txt

Energized Antipop-ups (47k): https://energized.pro/antipopads-re/adblock.txt

OTHER BLOCK LIST PROJECT LISTS:

Block List Project Ads (154k): https://blocklistproject.github.io/Lists/adguard/ads-ags.txt

Block List Project Crypto (23k): https://blocklistproject.github.io/Lists/adguard/crypto-ags.txt

Block List Project Malware (435k): https://blocklistproject.github.io/Lists/adguard/malware-ags.txt

Block List Project Phishing (190k): https://blocklistproject.github.io/Lists/adguard/phishing-ags.txt

Block List Project Ransomware (2k): https://blocklistproject.github.io/Lists/adguard/ransomware-ags.txt

Block List Project Tracking (15k): https://blocklistproject.github.io/Lists/adguard/tracking-ags.txt

Block List Project Scam (1k): https://blocklistproject.github.io/Lists/adguard/scam-ags.txt

MINIFIED/OPTIMIZED LISTS:

EasyList Minified (16k): https://easylist-downloads.adblockplus.org/easylist-minified.txt

EasyList Optimized (51k): https://filters.adtidy.org/extension/ublock/filters/101_optimized.txt

EasyPrivacy Minified (5k): https://easylist-downloads.adblockplus.org/easyprivacy-minified.txt

EasyPrivacy Optimized (30k): https://filters.adtidy.org/extension/ublock/filters/118_optimized.txt

AdGuard Base + EasyList Optimized (78k): https://filters.adtidy.org/extension/ublock/filters/2_optimized.txt

AdGuard Mobile Ads Optimized (11k): https://filters.adtidy.org/extension/ublock/filters/11_optimized.txt

AdGuard Tracking Protection Optimized (164k): https://filters.adtidy.org/extension/ublock/filters/3_optimized.txt

AdGuard Annoyances Optimized (48k): https://filters.adtidy.org/extension/ublock/filters/14_optimized.txt

Fanboy Annoyances Optimized (42k): https://filters.adtidy.org/extension/ublock/filters/122_optimized.txt

AdGuard Social Optimized (17k): https://filters.adtidy.org/extension/ublock/filters/4_optimized.txt

Fanboy's Social Minified (3k): https://easylist-downloads.adblockplus.org/fanboy-social-minified.txt

Fanboy's Social Optimized (7k): https://filters.adtidy.org/extension/ublock/filters/123_optimized.txt

```
**CHECK MY FILTER LISTS:** https://github.com/LexReek/adBlocklists

**PAGES WITH LIST AND SETTINGS RECOMMENDATIONS:**

https://12bytes.org/ublock-origin-suggested-settings/

https://adblockplus.org/subscriptions

https://adblockultimate.net/filters

https://avoidthehack.com/best-pihole-blocklists

https://blokada.org/api/v4/content/en/filters.txt

https://codeberg.org/celenity/BadBlock

https://codeberg.org/celenity/Phoenix/wiki/Content-Blocking

https://codeberg.org/celenity/ublock-origin-settings

https://divested.dev/pages/dnsbl

https://easylist.to/

https://energized.pro/

https://filterlists.com/

https://firebog.net/

https://github.com/AdguardTeam/FiltersRegistry/tree/master/filters

https://github.com/blocklistproject/Lists

https://github.com/celenityy/adguard-extension-settings

https://github.com/celenityy/adguard-home-settings

https://github.com/celenityy/BadBlock

https://github.com/celenityy/ublock-origin-settings

https://github.com/DandelionSprout/adfilt

https://github.com/EnergizedProtection/block

https://github.com/EnergizedProtection/EnergizedHosts

https://github.com/hagezi/dns-blocklists

https://github.com/knapah/uBlockOrigin-Filterlist

https://github.com/maravento/blackweb

https://github.com/ryanbr

https://github.com/StevenBlack/hosts

https://github.com/uBlockOrigin/uAssets/tree/master/filters

https://github.com/uBlockOrigin/uAssetsCDN

https://github.com/yokoffing/filterlists

https://kb.adguard.com/en/general/adguard-ad-filters

https://mdleom.com/about

https://oisd.nl/setup

https://tw3.gitlab.io/tw3filterlists/umatrix/

https://www.fanboy.co.nz/

https://www.fanboy.co.nz/regional.html

https://www.iblocklist.com/lists.php

https://www.kaggle.com/datasets/shivd24coder/clean-web-adblock-filters

https://zeltser.com/malicious-ip-blocklists/

https://help.kagi.com/orion/features/custom-blocklists.html

https://pastebin.com/nUSHUWXc

### 5.7. RECOMMENDED CONFIGURATIONS IN LOCALCDN:**

Block Google Fonts -> ❌ (This is already covered by Yokoffing's Block list of third-party fonts, which I recommend; leaving Google Fonts blocked here will also cause problems and breakages.)

In the Advanced tab, scroll down, click on uBlock and copy all the lines that appear. Then, open uBlock Origin, the "My Rules" panel, and paste into "Temporary Rules," click Save, and then Confirm.

Source: [Celenity](https://github.com/celenityy/ublock-origin-settings?#localcdn---advanced).

### 5.8. USER SCRIPTS RECOMMENDATIONS (FOR VIOLENT MONKEY):

UserScripts are small pieces of code written in JavaScript that modify web pages by adding useful functions. To use them, you will need an extension called a userscript manager . We recommend using ViolentMonkey , which is open source. Scripts can be downloaded from internet repositories, but this requires a high degree of trust in the developer, as they may be compromised. Generating fingerprinting can increase the attack surface and present risks to privacy and security. Below are some recommendations focused on security and privacy (emphasis on the first three):

```
AdGuard Extra - blocks ads in difficult cases, when the usual filter-based approach is not enough.
https://github.com/AdguardTeam/AdGuardExtra#userscript

Don't track me Google - removes the link tracking feature from Google search results. This speeds up the loading of search results and allows you to right-click or tap to copy the URL link.
https://github.com/Rob--W/dont-track-me-google

AdGuard Disable AMP - Disables AMP (Accelerated Mobile Pages) on the Google search results page (there is also an adblock filter for this purpose, which would eliminate the need to use this script).
https://github.com/AdguardTeam/DisableAMP#how-to-install

AdGuard PopUp Blocker - Blocks unwanted pop-up ad windows.
https://github.com/AdguardTeam/PopupBlocker#installation

AdsBypasser - Blocks countdown ads, intermediate continue pages, and pop-up ad windows.
https://adsbypasser.github.io

AntiAdware - Blocks the download of unwanted applications (forced download accelerators, managers, and adware) when downloading from supported websites.
https://github.com/HandyUserscripts/AntiAdware#installation

tinyShield - Blocks ads from AdShield and anti-adblockers and bypasses AdShield integrity verification (useful for Korean, Japanese, and some international websites).
https://github.com/List-KR/tinyShield

```
Source: [AdGuard](https://adguard.com/kb/general/extensions/) and [Awesome-Userscripts](https://github.com/awesome-scripts/awesome-userscripts).

### 5.9. RECOMMENDED SETTINGS IN CANVASBLOCKER:
After installing CanvasBlocker, an initial configuration screen will open; click on all four "Apply" buttons.
Copy the file below into Notepad and save it as “CanvasBlocker - settings.json”:

```
{
"logLevel": 1,
"urlSettings": [],
"hiddenSettings": {
"protectAudio": true,
"protectedAPIFeatures": true
},
"expandStatus": {
"protectNavigator": true,
"section_notifications": false,
"protectAudio": true,
"protectTextMetrics": false
},
"displayHiddenSettings": true,
"whiteList": "",
"sessionWhiteList": "",
"blackList": "",
"blockMode": "fake",
"protectedCanvasPart": "everything",
"minFakeSize": 10,
"maxFakeSize": 0,
"rng": "persistent",
"protectedAPIFeatures": {
"readPixels @ canvas": false,
"getParameter @ canvas": false,
"getExtension @ canvas": false
},
"useCanvasCache": true,
"ignoreFrequentColors": 3,
"minColors": 3,
"fakeAlphaChannel": false,
"webGLVendor": "",
"webGLRenderer": "",
"webGLUnmaskedVendor": "",
"webGLUnmaskedRenderer": "",
"persistentRndStorage": "",
"persistentIncognitoRndStorage": "",
"storePersistentRnd": false,
"persistentRndClearIntervalValue": 0,
"persistentRndClearIntervalUnit": "days",
"lastPersistentRndClearing": 1746443757258,
"sharePersistentRndBetweenDomains": false,
"askOnlyOnce": "individual",
"askDenyMode": "block",
"showCanvasWhileAsking": true,
"showNotifications": false,
"highlightPageAction": "none",
"highlightBrowserAction": "color",
"displayBadge": false,
"storeNotificationData": false,
"storeImageForInspection": false,
"ignoreList": "",
"ignoredAPIs": {},
"showCallingFile": false,
"showCompleteCallingStack": false,
"enableStackList": false,
"stackList": "",
"protectAudio": false,
"audioFakeRate": "100",
"audioNoiseLevel": "minimal",
"useAudioCache": true,
"audioUseFixedIndices": true,
"audioFixedIndices": "14",
"historyLengthThreshold": 2,
"protectWindow": false,
"allowWindowNameInFrames": false,
"protectDOMRect": true,
"domRectIntegerFactor": 4,
"protectSVG": true,
"protectTextMetrics": true,
"blockDataURLs": true,
"protectNavigator": false,
"navigatorDetails": {},
"protectScreen": true,
"screenSize": "",
"fakeMinimalScreenSize": true,
"displayAdvancedSettings": true,
"displayDescriptions": true,
"theme": "auto",
"dontShowOptionsOnUpdate": false,
"disruptSessionOnUpdate": false,
"updatePending": false,
"isStillDefault": false,
"storageVersion": 1
}
```

Open the settings in the General tab and scroll down until you find “CanvasBlocker settings export”, click load and select the saved file.
Source: [Chef-koch](https://chef-koch.bearblog.dev/firefox-hardened-canvasblocker-config/)

### 6. ADVANCED FIREFOX SETTINGS:

The configurations explained below. They can be used in Firefox or its variants.
However, for browser options pre-hardened (like LibreWolf, Mullvad, Tor Browser, etc) no I recommend such modifications, unless what own knowledge advanced Regarding the implications .

### 6.1. ABOUT:CONFIG

Typing **about:config** in the address bar will open the Firefox internal settings page, listed as "preferences," which can be meticulously configured, changing the appearance, security, functionality, etc.

To modify an existing preference, search for its name and double-click on it. If it's a boolean value, it will be inverted; if it's an integer or string value, a field will open to change the value.
 
To create a preference, right-click > “New preference” > select the type, type the entry name, and then set its value.

There are three “types” of inputs:
- Boolean – only accepts the values true or false, and is used to turn a setting on or off.
- Integer – accepts any integer, used to define the value of a given setting (for example, the maximum amount of memory used).
- String – accepts values composed of letters and/or numbers, used to store some information (for example, the homepage address).

### 6.2. USER.JS

An easier way to change numerous preferences is by creating a user settings file (user.js). This way, every time Firefox starts, it loads the entries in the file and automatically adds them to your settings, which are stored in the user preferences file (prefs.js).

To create a settings file, simply copy the desired preferences from the table below and paste them into Notepad, then save it as "user.js" in the profile folder located at:
“C:\Users\<Name_user>\AppData\Roaming\Mozilla\Firefox\Profiles\<something>.default”
Note: To find this folder, hidden folders must be displayed (open Windows Explorer > Tools menu > Folder Options > View tab > check Show hidden files and folders).

Below is an example of a user.js file, where each line corresponds to a preference/configuration. Lines beginning with two backslashes (\\) contain a brief description of the function of the following lines.

```
// Prevents websites from altering or hiding browser elements (such as toolbars, window size, etc.)
user_pref("dom.disable_window_move_resize", true);
user_pref("dom.disable_window_open_feature.close", true);
user_pref("dom.disable_window_open_feature.location", true);
user_pref("dom.disable_window_open_feature.menubar", true);
user_pref("dom.disable_window_open_feature.minimizable", true);
user_pref("dom.disable_window_open_feature.personalbar", true);
user_pref("dom.disable_window_open_feature.resizable", true);
user_pref("dom.disable_window_open_feature.scrollbars", true);
user_pref("dom.disable_window_open_feature.status", true);
user_pref("dom.disable_window_open_feature.titlebar", true);
user_pref("dom.disable_window_open_feature.toolbar", true);
user_pref("dom.disable_window_showModalDialog", true);
user_pref("dom.disable_window_status_change", true);
user_pref("dom.disable_window_flip", true);

// Open links only in a new tab in the current window.
user_pref("browser.link.open_external", 3);
user_pref("browser.link.open_newwindow", 3);
user_pref("browser.link.open_newwindow.restriction", 0);

// Block pop-ups initiated by plugins (such as Java and Flash)
user_pref("privacy.popups.disable_from_plugins", 2);

// Remove cookie warning banners
user_pref("cookiebanners.service.mode.privateBrowsing", 1);

// Cookie settings for security
user_pref("network.cookie.cookieBehavior", 5);
user_pref("security.cert_pinning.enforcement_level", 2); // Habilitar Pinning Strict (PKP - Public Key Pinning) = pode ocasionar problemas com antivírus, neste caso mude para 1
user_pref("network.cookie.lifetimePolicy", 2); // Se definir como 3 os cookies serão armazenados pelo número de dias definidos em network.cookie.lifetime.days
user_pref("network.cookie.lifetime.days", 15);

// Enable ETP (Enhanced Tracking Protection) in strict mode to enable TCP (Total Cookie Protection):
user_pref("browser.contentblocking.category", "strict");

// Activate state partitioning of service workers
user_pref("privacy.partition.serviceWorkers", true);

// Enable APS (Always Partitioning Storage
user_pref("privacy.partition.always_partition_third_party_non_cookie_storage", true);
user_pref("privacy.partition.always_partition_third_party_non_cookie_storage.exempt_sessionstorage", true);

// Prevents automatic reloading on websites (auto-refresh)
user_pref("accessibility.blockautorefresh", true);

// Prevents websites from blocking the right-click button
user_pref("dom.event.contextmenu.enabled", false);

// Prevents websites from blocking copying/accessing clipboard content
user_pref("dom.event.clipboardevents.enabled", false);

// AdGuard 's DoH DNS resolver with filtering
user_pref("network.trr.mode", 3);
user_pref("network.trr.uri", https://dns.adguard-dns.com/dns-query);

// Disable automatic DNS preloading
user_pref("network.dns.disablePrefetch", true);
user_pref("network.dns.disablePrefetchFromHTTPS", true);

// Disable automatic link preloading
user_pref("network.prefetch-next", false);
user_pref("network.predictor.enabled", false);
user_pref("network.http.speculative-parallel-limit", 0);
user_pref("browser.places.speculativeConnect.enabled", false);

// Disable automatic page preloading in newtab.
user_pref("browser.newtab.preload", false);

// Disable automatic preloading of the website you are typing in the address bar.
user_pref("browser.urlbar.speculativeConnect.enabled", false);

// Disable search suggestions
user_pref("browser.search.suggest.enabled", false);
user_pref("browser.urlbar.suggest.searches", false);

// Disable domain guessing in the address bar
user_pref("browser.fixup.alternate.enabled", false);

// Disable speculative connections from the address bar.
user_pref("browser.urlbar.speculativeConnect.enabled", false);

// Disable contextual suggestions in the address bar.
user_pref("browser.urlbar.quicksuggest.scenario", "history");
user_pref("browser.urlbar.quicksuggest.enabled", false);
user_pref("browser.urlbar.suggest.quicksuggest.nonsponsored", false);
user_pref("browser.urlbar.suggest.quicksuggest.sponsored", false);

// Show full URL
user_pref("browser.urlbar.trimURLs", false);

// Disable form autofill
user_pref("browser.formfill.enable", false);
user_pref("extensions.formautofill.addresses.enabled", false);
user_pref("extensions.formautofill.available, "off");
user_pref("extensions.formautofill.creditCards.available", false);
user_pref("extensions.formautofill.creditCards.enabled", false);
user_pref("extensions.formautofill.heuristics.enabled", false);

// Disable saving passwords
user_pref("signon.rememberSignons", false);
user_pref("signon.autofillForms", false);
user_pref("signon.formlessCapture.enabled", false);

// Strengthen your defenses against potential phishing credentials
user_pref("network.auth.subresource-http-auth-allow", 1);

// Always start in Private Window
user_pref("browser.privatebrowsing.autostart", true);

// Removes error when using VPN extension
user_pref("security.OCSP.require", false);

// Same zoom for all sites (instead of one for each site)
user_pref("browser.zoom.siteSpecific", false);

// Enables spell checking for single-line text.
user_pref("layout.spellcheckDefault", 2);

// Getting rid of "Do you really want to leave this site?" pop-ups.
user_pref("dom.disable_beforeunload", true);

// Block popup windows
user_pref("dom.disable_open_during_load", true);

// Limit events that cause popups
user_pref("dom.popup_allowed_events", "click dblclick mousedown pointerdown");

// Increases the write interval of recovery.js to extend the lifespan of the SSD.
user_pref("browser.sessionstore.interval", 300000);

// Do not warn when closing tabs/guides
user_pref("browser.tabs.warnOnClose", false);
user_pref("browser.tabs.warnOnCloseOtherTabs", false);

// Disable checking if Firefox is the primary browser.
user_pref("browser.shell.checkDefaultBrowser", false);

// Always ask where to save.
user_pref("browser.download.useDownloadDir", false);

// Disable adding downloads to the system's "recent documents" list.
user_pref("browser.download.manager.addToRecentDocs", false);

// Set page to "home page"
user_pref("browser.newtab.url", "https://duckduckgo.com/");

// Forcing the installation of incompatible add-ons (I don't know if this still works)
user_pref("xpinstall.signatures.required", false);
user_pref("extensions.checkCompatibility", false);

// Disable disk caching (does it in RAM)
user_pref("browser.cache.disk.enable", false);

// Disable extra session data storage.
user_pref("browser.sessionstore.privacy_level", 2);

// Disable resume session after crash
user_pref("browser.sessionstore.resume_from_crash", false);

// Disable page thumbnail collection
user_pref("browser.pagethumbnails.capturing_disabled", true);

// Disable favicons in the profile folder.
user_pref("browser.shell.shortcutFavicons", false);

// Delete temporary files opened with external applications
user_pref("browser.helperApps.deleteTempFileOnExit", true);

// Prevent accessibility services from starting in the browser.
user_pref("accessibility.force_disabled", 1);

// Do not select the space next to a word when double-clicking it.
user_pref("layout.word_select.eat_space_to_next_word", false);

// Enable pipelining ( tweak )
user_pref("network.http.pipelining", true);
user_pref("network.http.pipelining.abtest", false);
user_pref("network.http.pipelining.aggressive", true);
user_pref("network.http.pipelining.max-optimistic-requests", 3);
user_pref("network.http.pipelining.maxrequests", 12);
user_pref("network.http.pipelining.maxsize", 300000);
user_pref("network.http.pipelining.read-timeout", 60000);
user_pref("network.http.pipelining.reschedule-on-timeout", true);
user_pref("network.http.pipelining.reschedule-timeout", 15000);
user_pref("network.http.pipelining.ssl", true);
user_pref("network.http.proxy.pipelining", true);

// Reduces RAM usage when minimized (recommended only if you have limited RAM)
user_pref("config.trim_on_minimize", true);

// Enable Firefox privacy protections.
user_pref("privacy.fingerprintingProtection", true);
user_pref("privacy.globalprivacycontrol.was_ever_enabled", true);
user_pref("privacy.trackingprotection.cryptomining.enabled", true);
user_pref("privacy.trackingprotection.enabled", true);
user_pref("privacy.trackingprotection.fingerprinting.enabled", true);
user_pref("privacy.trackingprotection.socialtracking.enabled", true);

// Enable GPC (Global Privacy (Control ) - signals to websites that you object to the sale and sharing of your data. GPC came to replace DNT (Do Not Track).
user_pref("privacy.globalprivacycontrol.enabled", true);
user_pref("privacy.globalprivacycontrol.functionality.enabled", true);
user_pref("privacy.globalprivacycontrol.pbmode.enabled", true);

// Disable Geolocation
user_pref("geo.enabled", false);
user_pref("geo.wifi.logging.enabled", false);
user_pref("geo.wifi.uri", "");
user_pref("permissions.default.geo", 2);

// Disable Telemetry
user_pref("toolkit.telemetry.enabled", false);
user_pref("toolkit.telemetry.unified", false);

// Disable other telemetry services.
user_pref("toolkit.telemetry.server", "data:,");
user_pref("toolkit.telemetry.archive.enabled", false);
user_pref("toolkit.telemetry.newProfilePing.enabled", false);
user_pref("toolkit.telemetry.shutdownPingSender.enabled", false);
user_pref("toolkit.telemetry.updatePing.enabled", false);
user_pref("toolkit.telemetry.bhrPing.enabled", false);
user_pref("toolkit.telemetry.firstShutdownPing.enabled", false);
user_pref("toolkit.telemetry.coverage.opt-out", true);
user_pref("toolkit.coverage.opt-out", true);
user_pref("toolkit.coverage.endpoint.base", "");
user_pref("browser.ping-centre.telemetry", false);

// Disable Geographic Segmentation
user_pref("browser.search.countryCode", "NOS");
user_pref("browser.search.geoSpecificDefaults", false);
user_pref("browser.search.geoSpecificDefaults.url", "");
user_pref("browser.search.geoip.url", "");
user_pref("browser.search.region", "NOS");

// Disable Crash Reporting
user_pref("breakpad.reportURL", "");
user_pref("browser.tabs.crashReporting.sendReport", false);

// Disable collection of information about newtab (telemetry)
user_pref("browser.newtabpage.directory.ping", "");
user_pref("browser.newtabpage.directory.source", "");

// From here on, more advanced knowledge is required. Many entries disable APIs, which enhances browser privacy but can cause websites to break.

// Prevent your browser from telling websites your language locale
user_pref("intl.locale.matchOS", false);
user_pref("general.useragent.locale", "NOS");

// Disable sending of referrer header (reports originating site)
user_pref("network.http.sendRefererHeader", 0);
user_pref("network.http.sendSecureXSiteReferrer", false);

// Disable DNS proxy redirection
user_pref("network.proxy.socks_remote_dns", true);

// Punycode
user_pref("network.IDN_show_punycode", true);

// Disable IPv6
user_pref("network.dns.disableIPv6", true);

// Disable Gio protocols - potential proxy bypass
user_pref("network.gio.supported-protocols", "");

// Disable use of UNC ( Uniform) Naming Convention) - prevents proxy bypass :
user_pref("network.file.disable_unc_paths", true);

// Disable Heartbeat
user_pref("browser.selfsupport.url", "");

// Disable Health Report
user_pref("datareporting.healthreport.about.reportUrl", "");
user_pref("datareporting.healthreport.about.reportUrlUnified", "");
user_pref("datareporting.healthreport.documentServerURI", "");
user_pref("datareporting.healthreport.infoURL", "");
user_pref("datareporting.healthreport.logging.consoleEnabled", false);
user_pref("datareporting.healthreport.service.enabled", false);
user_pref("datareporting.healthreport.uploadEnabled", false);
user_pref("datareporting.policy.dataSubmissionEnabled", false);
user_pref("datareporting.policy.dataSubmissionEnabled.v2", false);

// Disable Safe Browsing (this checks if the URL is malicious in Google's databases, which generated some tracking until 2011. There have been improvements to prevent this from happening, but it is still recommended to disable it)
user_pref("browser.safebrowsing.downloads.enabled", false);
user_pref("browser.safebrowsing.downloads.remote.enabled", false);
user_pref("browser.safebrowsing.downloads.remote.url", "");
user_pref("browser.safebrowsing.enabled", false);
user_pref("browser.safebrowsing.malware.enabled", false);
user_pref("browser.safebrowsing.phishing.enabled", false);
user_pref("browser.safebrowsing.blockedURIs.enabled", false);
user_pref("browser.safebrowsing.allowOverride", false);

// SafeBrowsing update search
user_pref("browser.safebrowsing.provider.google4.gethashURL", "");
user_pref("browser.safebrowsing.provider.google4.updateURL", "");
user_pref("browser.safebrowsing.provider.google.gethashURL", "");
user_pref("browser.safebrowsing.provider.google.updateURL", "");
user_pref("browser.safebrowsing.provider.google4.dataSharingURL", "");
user_pref("browser.safebrowsing.downloads.remote.block_potentially_unwanted", false);
user_pref("browser.safebrowsing.downloads.remote.block_uncommon", false);

// Disable HTML5 Video statistics
user_pref("media.video_stats.enabled", false);

// Disable metadata verification on installed add-ons
user_pref("extensions.getAddons.cache.enabled", false);

// Disable Pocket extension
user_pref("browser.pocket.enabled", false);
user_pref("extensions.pocket.enabled", false);

// Disable Screenshots extension
user_pref("extensions.Screenshots.disabled", true);

// Disable PDF scripting
user_pref("pdfjs.enableScripting", false);

// Define extensions to work in restricted domains
user_pref("extensions.enabledScopes", 5);
user_pref("extensions.webextensions.restrictedDomains", "");
user_pref("extensions.postDownloadThirdPartyPrompt", false); // Sempre exibir o prompt de instalação

// Disable DRM (streaming services will not work or will play at reduced quality)
user_pref("media.eme.enabled", false);
user_pref("browser.eme.ui.enabled", false);
user_pref("media.gmp-widevinecdm.enabled", false);
user_pref("media.gmp-widevinecdm.visible", false);

// Disable SVG
user_pref("svg.disabled", true);

// Disabling WebGL (Web Graphics Library) may break gaming websites .
user_pref("webgl.disabled", true);

// Disable WebGPU
user_pref("dom.webgpu.enabled", false);

// Disable WebRTC ( IP leaks)
user_pref("media.peerconnection.enabled", false);

// Reinforce disabling WebRTC
user_pref("media.peerconnection.ice.default_address_only", true);
user_pref("media.peerconnection.ice.proxy_only_if_behind_proxy", true);
user_pref("media.peerconnection.ice.no_host", true);

// Disable Beacon
user_pref("beacon.enabled", false);

// Disable WebAssembly - WASM
user_pref("javascript.options.wasm", false);

// Always use secure negotiation methods (occasionally some sites may display a "secure connection failed" error).
user_pref("security.ssl.require_safe_negotiation", true);

// cross-site referrals.
user_pref("network.http.referer.XOriginPolicy", 1); // 2 para maior segurança, mas quebra muitos sites
user_pref("network.http.referer.XOriginTrimmingPolicy", 2);

// Activate Fingerprinting Advanced Protection (RFP) (may be aggressive for some sites)
user_pref("privacy.resistFingerprinting", true);

// Enable letterboxing (borders) in the window to prevent monitor-sized fingerprinting .
user_pref("privacy.resistfingerprinting.letterboxing", true);
user_pref("privacy.resistFingerprinting.letterboxing.dimensions", "800x600, 1000x1000, 1600x900"); //define o(s) tamanho(s) de tela

// Additional entries to mitigate fingerprinting
user_pref("privacy.resistFingerprinting.autoDeclineNoUserInputCanvasPrompts", true);
user_pref("privacy.resistFingerprinting.block_mozAddonManager", true);
user_pref("privacy.resistFingerprinting.exemptedDomains", "*.example.invalid");
user_pref("privacy.resistFingerprinting.jsmloglevel", "Warn");
user_pref("privacy.resistFingerprinting.randomDataOnCanvasExtract", true);
user_pref("privacy.resistFingerprinting.reduceTimerPrecision.jitter", true);
user_pref("privacy.resistFingerprinting.reduceTimerPrecision.microseconds", 1000);
user_pref("privacy.resistFingerprinting.target_video_res", 480);
user_pref("privacy.resistFingerprinting.testGranularityMask", 0);
user_pref("services.sync.prefs.sync.privacy.resistFingerprinting.reduceTimerPrecision.jitter", true);
user_pref("services.sync.prefs.sync.privacy.resistFingerprinting.reduceTimerPrecision.microseconds", true);
user_pref("privacy.window.maxInnerWidth",  1600);
user_pref("privacy.window.maxInnerHeight", 900);
user_pref("browser.display.use_system_colors", false);
user_pref("browser.startup.blankWindow", false);

// Enable location sensor API (referring to the RFP)
user_pref("device.sensors.enabled", false);
user_pref("device.sensors.motion.enabled", false);
user_pref("device.sensors.orientation.enabled", false);

// Disable mozAddonManager Web API (referring to RFP)
user_pref("privacy.resistFingerprinting.block_mozAddonManager", true);

// Enable containers
user_pref("privacy.userContext.enabled", true);

// Isolate cookies
user_pref("privacy.firstparty.isolate", true);

// Prevent websites from tracking microphone and camera status.
user_pref("media.navigator.enabled", false);

// Prevent test connections (Firefox attempts to connect to Amazon and Akamai servers to test the browser)
user_pref("network.captive-portal-service.enabled", false);

// Enable Encrypted Client Hello (ECH)
user_pref("network.dns.echconfig.enabled", true);
user_pref("network.dns.http3_echconfig.enabled", true);

// It can be used to track visitor clicks.
user_pref("browser.send_pings", false);

// Prevent websites from obtaining your battery status.
user_pref("dom.battery.enabled", false);

Disable Activity Stream in new tabs
user_pref("browser.newtabpage.enabled", false);
user_pref("browser.newtab.preload", false);
user_pref("browser.newtabpage.activity-stream.feeds.telemetry", false);
user_pref("browser.newtabpage.activity-stream.telemetry", false);
user_pref("browser.newtabpage.activity-stream.feeds.snippets", false);
user_pref("browser.newtabpage.activity-stream.feeds.section.topstories", false);
user_pref("browser.newtabpage.activity-stream.section.highlights.includePocket", false);
user_pref("browser.newtabpage.activity-stream.feeds.discoverystreamfeed", false);
user_pref("browser.newtabpage.activity-stream.showSponsored", false);
user_pref("browser.newtabpage.activity-stream.showSponsoredTopSites", false);
user_pref("browser.newtabpage.activity-stream.default.sites", "");

// Use the Mozilla geolocation service instead of Google.
user_pref("geo.provider.network.url", "https://location.services.mozilla.com/v1/geolocate?key=%MOZILLA_API_KEY%");

// Disable the use of the operating system's geolocation service.
user_pref("geo.provider.ms-windows-location", false); // Windows
user_pref("geo.provider.use_corelocation", false); // macOS
user_pref("geo.provider.use_gpsd", false); // Linux
user_pref("geo.provider.use_geoclue", false); // Linux

// Disable region updates.
user_pref("browser.region.network.url", "");
user_pref("browser.region.update.enabled", false);

// Set the language to display web pages
user_pref("intl.accept_languages", "en-US, en"
user_pref("javascript.use_us_english_locale", true);

// Disable add-on recommendations (uses Google Analytics )
user_pref("extensions.getAddons.showPane", false);
user_pref("extensions.htmlaboutaddons.recommendations.enabled", false);
user_pref("browser.discovery.enabled", false);

// Disable studies
user_pref("app.shield.optoutstudies.enabled", false);
user_pref("app.normandy.enabled", false);
user_pref("app.normandy.api_url", "");

// Disable Captive Portal Detection
user_pref("captivedetect.canonicalURL", "");
user_pref("network.captive-portal-service.enabled", false);

// Disable network connection checks.
user_pref("network.connectivity-service.enabled", false);

// Remove special permissions for certain Mozilla domains.
user_pref("permissions.manager.defaultsUrl", "");

// Enable HTTPS-only mode on all windows.
user_pref("dom.security.https_only_mode", true);

// Disable sending HTTP requests to verify HTTPS support by the server.
user_pref("dom.security.https_only_mode_send_http_background_request", false);

// Display advanced information about insecure connection warning pages
user_pref("browser.xul.error_pages.expert_bad_cert", true);

// Disable TLS 1.3 0-RTT (Round-trip time)
user_pref("security.tls.enable_0rtt_data", false);

// Define OCSP to terminate the connection when a CA is not validated
user_pref("security.OCSP.require", true);

// Disable SHA-1 certificates
user_pref("security.pki.sha1_enforcement_level", 1);

// Enable CRLite
user_pref("security.remote_settings.crlite_filters.enabled", true);
user_pref("security.pki.crlite_mode", 2);

// Clear history, cookies, and site data when Firefox closes.
user_pref("network.cookie.lifetimePolicy", 2);
user_pref("privacy.sanitize.sanitizeOnShutdown", true);
user_pref("privacy.clearOnShutdown.cache", true);
user_pref("privacy.clearOnShutdown.cookies", true);
user_pref("privacy.clearOnShutdown.downloads", true);
user_pref("privacy.clearOnShutdown.formdata", true);
user_pref("privacy.clearOnShutdown.history", true);
user_pref("privacy.clearOnShutdown.offlineApps", true);
user_pref("privacy.clearOnShutdown.sessions", true);
user_pref("privacy.clearOnShutdown.sitesettings", false);
user_pref("privacy.sanitize.timeSpan", 0); 
```

### 6.3. ARKENFOX

There are countless websites on the internet that teach about modifying configuration entries, and others that provide ready-made configuration files (user.js), such as [BetterFox](https://github.com/yokoffing/Betterfox), [Brainfucksec](https://brainfucksec.github.io/firefox-hardening-guide), [FFprofile](https://ffprofile.com/), and [Narsil](https://git.nixnet.services/Narsil/desktop_user.js). and [Pyllyukko](https://github.com/pyllyukko/user.js). However, the biggest highlight is the [ArkenFox project](https://github.com/arkenfox/user.js/), where the community has been constantly improving a configuration file model (user.js) focused on privacy and security, but minimally impacting browser usability (although, unfortunately, problems do occur on some websites).

**Check my user.js file:** https://raw.githubusercontent.com/LexReek/user.js/refs/heads/main/user.js

**ArkenFox installation procedure:**

1. With Firefox installed, download the file available at:
https://github.com/arkenfox/user.js/blob/master/scratchpad-scripts/arkenfox-cleanup.js

2. If you wish, back up your profile for security;

Note: To find the profile folder, open Firefox, type “about:support” in the address bar, press Enter, search for “Profile Folder” and click “Open Folder”. Make a copy of the "prefs.js" file.

3. Disconnect from the internet;

4. Open the downloaded script with Notepad and scroll down a bit until you see the list of preferences. Remove the comma at the end of the last preference that appears above the following warning line:

/* IMPORTANT: last active pref must not have a trailing comma */

5. Copy all the contents of the opened file;

6. In Firefox, type the following into the address bar and press Enter:

about:config

7. Press Ctrl+Shift+K to open the Web Console;

8. Type “allow paste” and press Enter;

9. Copy and press Enter;

10. Restart Firefox and re-enable the connection;

11. Access the following address:

https://github.com/arkenfox/user.js/tree/master

12. Download the following files:

- prefsCleaner.bat (for Windows)

- prefscleaner.sh (for Linux)

- updater.bat (for Windows)

- updater.sh (for Linux)

- user.js

Note: To download the file, click on its name and then on the “Download raw file” button that appears near the upper right corner. Then, go back and repeat with each file.

13. If you have any configuration entries that you want to use with ArkenFox (such as those shown in the previous table), save them using Notepad with the following name:

user-overrides.js

13.a. You can consult the user-overrides.js templates from [12bytes](https://codeberg.org/12bytes/Firefox-user.js-supplement/raw/branch/master/user-overrides.js) ([source](https://12bytes.org/the-firefox-privacy-guide-for-dummies/)) and [yokoffing](https://raw.githubusercontent.com/yokoffing/Betterfox/refs/heads/main/personal/user-overrides.js).

14. In Firefox, type the following into the address bar and press Enter:

about:support

15. On the page that opens, look for “Profile folder” and click on “Open folder”;

16. Place the files from steps 12 and 13 in the folder that opened;

17. Close Firefox;

18. Right-click on the “Updater.bat” file, then select “Run as administrator”. In the window that opens, type “Y” and wait for it to finish. If it offers to run “prefsCleaner.bat”, type “Y”.

19. If not, right-click on the “prefsCleaner.bat” file, then select “Run as administrator” and wait for it to finish.

**ArkenFox update procedure:**

1. Check your ArkenFox version by accessing your profile folder (as in steps 13 and 14) and opening the “user.js” file with Notepad;

2. Compare with the ArkenFox version available at:

https://raw.githubusercontent.com/arkenfox/user.js/refs/heads/master/user.js

3. Whenever the ArkenFox version on the website is the latest, download the user.js file and place it in your profile folder (as in steps 11, 13 and 14);

4. If you want to add any configuration entries, add them to the “user-overrides.js” file (as in step 12);

5. Repeat steps 16, 17 and 18.

### 7. RECOMMENDED VPN PROVIDERS:

A VPN (Virtual Private Network) provides a secure and encrypted connection for data traffic between the user and the VPN server, preventing the network (public or private), your internet service provider (ISP), or third parties from understanding the content of the data sent and received. Furthermore, it hides your online identity (IP address and location), as others will see the VPN server as the data source or end user.

When using a VPN, take some precautions: opt for well-known and audited companies (these are usually paid options); prefer providers with their own dedicated servers, rather than rented or shared ones; choose a server that is closer to you to reduce latency; VPN providers encrypt DNS requests through the VPN itself, and some have their own DNS resolvers, reducing the need to choose a private DNS resolver; use a secure protocol such as OpenVPN or WireGuard (WireGuard is more secure, simpler, and faster, but it is still recent and not as mature as OpenVPN ); avoid servers and companies located in countries whose laws do not guarantee minimum protection of data and cryptographic keys, that have authoritarian regimes, or strong monitoring/intelligence/espionage programs (see the list of countries not recommended in section 7.1).

The VPN providers listed below have at least the following characteristics: externally audited no-logs privacy policy, open source code, headquarters outside the nine eyes and external collaborators, registration with minimal information (maximum email), accepts cryptocurrency payments, supports connections with strong OpenVPN encryption protocols (with SHA-256 authentication) and WireGuard, supports multi-hop, has an Android option, kill-switch function (disables connections outside the VPN), provides Perfect Forward Secrecy (PFS).

| Provider | Headquarters | Countries | Servers | Structure | Free option | Remote Door Forwarding | IPv6 | Supported encryption protocols | Obfuscation Protocol[^20] | Record |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Proton](https://addons.mozilla.org/pt-BR/firefox/addon/proton-vpn-firefox-extension/)[^11] | Switzerland | 112 | 6638 | Owned + rented | Yes[^15] | Partial[^16] | No[^17] | OpenVPN , WireGuard and IKEv2/IPSec[^19] | Stealth | E-mail |
| Mullvad[^12] | Sweden | 47 | 695 | Owned + rented | No | No | Yes | OpenVPN and WireGuard | ShadowSocks + v2ray[^21] | Anonymous |
| IVPN[^13] | Gibraltar[^14] | 31 | 77 | Rented | No | No | Yes[^18] | OpenVPN and WireGuard | v2ray or Obfsproxy[^22] | Anonymous |

[^11]: Proton uses servers with disk encryption, which are themselves "Secure Core" located in data centers in Switzerland, Iceland, and Sweden; Tor servers allow access to .onion sites; with VPN Accelerator that promises to increase connection stability and speed by up to 400%; with filtering of ads, trackers, and malicious domains (NetShield); it also grants access to other company services.
[^12]: Mullvad uses diskless servers (depending on the choice); promises VPN tunnels resistant to quantum computing; allows access to the Mullvad Leta search engine.
[^13]: IVPN uses rented bare-metal servers with secure IPMI access, reinstalled from scratch and with LUKS encrypted disks; filtering of ads, trackers and malicious domains; firewall against DNS, IPv6 and WebRTC leaks.
[^14]: Gibraltar is an overseas territory of the United Kingdom (Five Eyes) and we were unable to ascertain whether the data/key legislation of this country is the same as that of the United Kingdom or independent.
[^15]: Proton offers a free option, with modest speed and connections to a limited number of servers/countries, without the possibility of choice and generally with undesirable locations.
[^16]: Proton supports remote port forwarding only via NAT-PMP with 60-second lease times. This is easily accessible in the Windows application, but on other systems you will need to run your own NAT-PMP client. Torrent applications generally offer native support for NAT-PMP.
[^17]: is adding IPv6 support; for now, only the Linux version and the browser extension support it.
[^18]: IVPN allows you to connect to services that use IPv6, but it does not allow the user to connect from a device using an IPv6 address.
[^19]: The IKEv2/IPSec encryption protocol is faster, more stable, and compatible with mobile devices, but less secure.
[^20]: The obfuscation protocol is an additional protocol used in case the VPN is blocked, providing greater resistance against censorship.
[^21]: ShadowSocks + v2ray is more resistant against firewalls with Deep Packet Inspections that attempt to block VPNs (such as in China).
[^22]: v2ray ( VMess + QUIC or VMess + TCP) or Obfsproxy (TCP). QUIC is more modern and can be faster, but TCP makes your data appear as normal HTTP traffic.

### 7.1. COUNTRIES NOT RECOMMENDED FOR SERVER LOCATION:

Some countries have strong intelligence programs that monitor data traffic, such as the US, UK, Japan, and Germany. However, these programs are frequently used for illegitimate espionage purposes.

Let's take the US as an example, where companies can be subpoenaed by security agencies to provide the cryptographic keys of a specific user(s) without justification or court order, and the companies are even prohibited from speaking about the matter. Thus, the government secretly forces companies to transform their services (whether VPN, messaging, etc. ) into espionage tools. The same thing happens in the United Kingdom.

Therefore, VPN companies adopt a legal tactic, which consists of publishing a document called a "warrant canary" monthly, indicating that they have not received a secret court order up to that point. Therefore, if the company stops issuing this document, it means that they have received a secret court order.

Furthermore, the US always prioritizes the country's interests, even if this sometimes means violating international treaties.

It is not even advisable for your traffic to pass through there, since the US government, mainly through the NSA (National Security Agency), maintains more than 27 intelligence programs known to be used for surveillance (mass espionage), including illegitimately, as evidenced by cases already discovered and reported in the international media.

In addition to being a signatory to international intelligence agreements such as the UK-USA and Five Eyes agreements, which have already been caught being used for illegitimate espionage purposes, this is unfortunately not controllable, since many backbones pass through there and a large part of the world's data traffic passes through them.

Let's remember, for example, that in 2013 the international scandal erupted following the statements and documents leaked by Edward Snowden, proving US espionage against several countries.

Servers located in countries that closely monitor traffic or have authoritarian regimes, such as Russia and China, are also not recommended, as they often promote governmental and industrial espionage.

Avoid servers located in or owned by companies based in the following countries:

**Members of the Five Eyes (intelligence group):** Australia, Canada, USA, New Zealand, and the United Kingdom.

**Members of the Nine Eyes:** those listed above, plus Denmark, France, the Netherlands, and Norway.

**Members of the Fourteen Eyes:** those above, plus Germany, Belgium, Spain, Italy and Sweden.

**External collaborators of the Five Eyes program:** South Korea, Israel, Japan, and Singapore.

**Members of the SIGINT intelligence agreement Seniors of The Pacific:** Five Eyes, plus South Korea, France, India, Singapore, and Thailand.

**Members of the Shanghai Cooperation Organisation (SCO):** Kazakhstan, China, India, Iran, Pakistan, Kyrgyzstan, Russia, Tajikistan, and Uzbekistan.

**Laws require the provision of cryptographic keys in investigations:** South Africa, Germany, Antigua and Barbuda, Australia, USA, France, India, Ireland, Japan, New Zealand, Norway, United Kingdom, Russia.

**Restrictions on encryption, monitored traffic and/or censorship:** South Africa, Saudi Arabia, Bahamas, Bangladesh, Belarus, Cameroon, Cambodia, Kazakhstan, China, Colombia, North Korea, Cuba, Egypt, El Salvador, United Arab Emirates, Eritrea, Ethiopia, France, Ghana, India, Indonesia, Iran, Iraq, Israel, Malaysia, Malawi, Morocco, Mozambique, Myanmar, Oman, Pakistan, Russia, Senegal, Syria, Sudan, Thailand, Tunisia, Turkmenistan, Turkey, Uganda, Uzbekistan, Venezuela, Vietnam, Zambia.

**Countries with strong data protection laws and cryptographic keys:** Iceland, Switzerland, Panama, Costa Rica, Argentina, Poland, Czech Republic.

For detailed information on data laws and cryptographic keys, visit [privacidade.digital](https://www.privacidade.digital/provedores/) and [gp-digital.org](https://www.gp-digital.org/world-map-of-encryption/).

