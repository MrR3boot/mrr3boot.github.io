# Bug Bounty Hunting:

I prefer below available resources to succeed in Bug Bounty Hunting. I'll update this monthly with new techniques. Some of my bug bounty disclosures are available in [NullNews](http://nullnews.in)


## Platforms:


1. OpenBugBounty - (XSS/CSRF/IDOR)(Will accept report from any site)
2. BugCrowd
3. HackerOne
3. Cobalt.io
4. SynAck (Only invited researchers)
5. Other self hosted programs by different domains (Facebook Whitehat/Google VRP/ AT&T BB)

## Sub Domain Enumeration:


1. Enumall
2. Massdns
3. Sublist3r
4. Knock
5. VirusTotal
6. Shodan
7. Censys
8. Eye witness
9. [DNS Dumpster](https://dnsdumpster.com)
10. Google Dorking (site:sony.com -www)
11. Virus Total
12. [BugCrowd LevelUp](https://github.com/appsecco/bugcrowd-levelup-subdomain-enumeration)
13. DNSScan
14. Altdns
15. dns-parallel-prober
16. brutesubs
17. dirsearch
18. Aquatone

## Sub Domain Takeovers:


### Cloudfront Entries


1. ride.uber.com -  cname - cloudfront.com
2. xxxx.ubnt.com - cname - cloudfront.com

### AWS Misconfiguration


1. rubyci.s3.amazonaws.com
2. hackerone
3. uber
4. ubiquitinetworks
5. twitter etc.

### Default Pre-Installed Instances (Install-Update Credentials-Report)

[snapchat wordpress instance](https://hackerone.com/reports/274336)

### Unbouncepages

	- Cname: unbouncepages.com
	- Name: landing.udemy.com
	- Type: CNAME
	- Class: IN
	- TTL: 300

### Google Mapped Domains


	- 216.58.203.243    moderator.ubnt.com
	- 216.58.203.243    ghs.google.com
	- 216.58.203.243    ghs.l.google.com

## Automation:

1. autoSubTakeover [Github]
2. HostileSubBruteforcer
3. tko-subs
4. [Aws Extender](https://github.com/VirtueSecurity/aws-extender)

## Git - Recon:

1. gitrob
2. git-all-secrets
3. trufflehog
4. git-secrets
5. repo-supervisor

## API Enumeration from JS files:

[LinkFinder](https://github.com/GerbenJavado/LinkFinder)


## Acquisition Enumeration:

1. Crunchbase
2. [crt.sh](https://crt.sh)
3. [Censys](https://censys.io)
4. [Google Cert Repo](https://google.com/transparencyreport/https/ct)

## Content Discovery / Dir Bruting:

1. Wappalyzer
2. Retire.js
3. Built With
4. Vulners CVE Scanner
5. Patator
6. GoBuster
7. WPScan
8. CMSMap
9. Robots Disallowed
10. Burp Content Discovery
11. CMSExplorer
12. BlindElephant

## Content Management System Bugs:

1. Adobe Cold Fusion - (Famous RCE/Admin Salt Leakage/SQL Vuln)
2. Drupal CMS - (RCE)
3. Wordpress - (Plenty of Bugs)
4. Jenkins Automation Server

## Parameter Bruter:


1. Parameth
2. Back Slash Powered Scanner [Burp]

## XSS:


1. Polyglot
2. [FlashScanner](https://cure53.de/flashbang)
3. Common Input Vectors
4. Blind XSS Frameworks
	- Sleepy Puppy [Python]
	- XSS Hunter [Python]
	- Ground Control [Ruby/Smail]
5. [XSS MindMap](https://github.com/jackmasa)
6. XSS Hunter
7. Flash XSS (FFDec-ompiler, https://github.com/riusksk/FlashScanner, https://cure53.de/flashbang)

## Flash CSRF:

1. Target is Accepting on JSON format data and Blocking Cross Domain requests with CORS.

[GeekBoy POC](https://www.geekboy.ninja/blog/tag/flash-csrf/)

## SSTI:


1. [TPLMap](https://github.com/epinna/tplmap)

## SSRF:

1. Blind SSRF  
	- Google PoC.
	- Twitter PoC.
	- AWS metadata acquiring

2. Full SSRF

3. Out of Band

## OAuth/OpenRedirect:

Validation missing on State/Token/Code (Open Redirection on Google Acquisition)

## Fuzzing API:

 [Fuzzapi](https://github.com/Fuzzapi/fuzzapi)

## Logical Bugs:

1. Email Verification Check fails
2. Money Rounding Issues.

## Denial of Service:

1. Via Large input.
2. Via Images.
3. Via XLS/PDF/TXT.
4. Via Out of Band Blind SSRF.

## Android-Hunts:
1. Decompile app --> Look for /assets/  or /res/raw [AWS Prod Keys, Dev Leftovers]
2. Check for External Storage - Binary Info/Code without validation, Sandbox leak, GPS Info, Log Files
3. Detecting Read/Write External Storage - FileObserver
4. Obfuscation - Proguard
5. Webview Checks
	- setAllowContent
	- setAllowFileAccess
	- setAllowFileAccessFromURLs
	- setJavaScriptEnabled
	- setPluginState
	- setSavePassword  
6. JavaScriptInterfaces - "jsvar"   -------> RCE CVE-2012-6636 (SDK<=17 supported apps vulnerable)

## Payloads:

1. https://github.com/1N3
2. https://github.com/danielmiessler/SecLists

## Ref:

[Ron Chon Ref](https://github.com/ngalongc/bug-bounty-reference)
bugbounty.community/tools

