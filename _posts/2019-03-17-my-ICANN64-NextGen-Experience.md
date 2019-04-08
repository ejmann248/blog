---
layout: post
title: "My #ICANN64 Experience"
description: "A brief post discussing what I learnt and experienced during my time at ICANN64 in Kobe."
comments: false
keywords: "ICANN, Internet Governance"
---
At the beginning of March, I had the great opportunity to attend the ICANN64 Community Forum Meeting in Kobe, Japan as a [NextGen candidate](https://www.icann.org/news/announcement-2018-11-09-en) from Australia. The NextGen program aims to integrate newcomers to the ICANN ecosystem by funding and involving them in one of three annual ICANN meetings held throughout the year in various regions. For this meeting, the NextGen program had me presenting on Indonesian Data Protection Laws, attending every session and workshop I could get my hands on, and networking with some of the foremost minds in internet governance.

For those unaware of what ICANN does (such as me before I was chosen as part of the NextGen Program), ICANN is responsible for the maintenance of the [DNS](https://en.wikipedia.org/wiki/Domain_Name_System) (Domain Name System). This covers the translation from IP addresses to domain names, the domain name system itself and other peripheral systems. It sounds like a narrow focus, and in some respects it is, but it is a global system that connects over four billion users and as such is crucial to the governance of the internet.

Here I’ll be giving a review of some of the key points I drew out of the meeting and what I’ll be bringing back with me to Australia.

## Cyber-Security

One of the hot topics at this ICANN Meeting were the recent attacks on the DNS around the world which resulted in the United States Cyber Security Body issuing its first ever [Cybersecurity Emergency Directive](https://cyber.dhs.gov/ed/19-01/) ordering government bodies to take measures to secure their domains and DNS profiles. As has been discussed, many of these attacks were less attacks on the DNS itself but rather attacks on credentials or end users which allowed attackers to change DNS settings to redirect data or hijack website certificates.

Such attacks are outside the remit of ICANN, but it was still interesting to hear from the Security & Stability Advisory Committee of ICANN on Wednesday and Thursday about possible measures that organisations should take to prevent DNS attacks on end users and servers. These included multi-factor authentication, registry locking and constant domain monitoring. It was specifically noted that these sorts of attacks are not new, nor will they stop any time soon.

A more technical sort of attack discussed was that of Man-In-The-Middle (MTM) attacks on the DNS itself. To massively oversimplify it, this is an attack which occurs when resolving a given domain name and the request is hijacked by a malicious party to return a false IP address – meaning that you don’t see any difference with the web address, but you are being served a malicious website. This sort of attack plays off the historic nature of the DNS as the creators of the system did not foresee that request data could be interrupted or intercepted.

Luckily, a mitigation for this attack has been devised in the form of [DNSSEC](https://www.dnssec.net/) (DNS Security Extensions). DNSSEC uses digital signatures to ensure data is not tampered with between servers and provides certainty for resolvers insofar as they know the root key. DNSSEC has been available for several years now, and implementation is ongoing but not yet ubiquitous. Unless you run your own DNS there’s not much you need to worry about in terms of implementation, but you should be pressuring your domain provider to enable DNSSEC in their namespace.

Of note for Australians is that DNSSEC is enabled for the com.au and net.au root names but [not gov.au.](https://viewdns.info/dnssec/?domain=gov.au) This is strange, and I’ve since asked the Digital Transformation Agency ([currently responsible for the gov.au domain](https://www.dta.gov.au/blogs/discovery-playback-domain-name-administration)) if DNSSEC is on their radar because I’d certainly expect government domains to have the highest security possible.

![Fantastic Kobe](https://media.licdn.com/dms/image/C5112AQHqGkWclS9TLQ/article-inline_image-shrink_1500_2232/0?e=1560384000&v=beta&t=vpzlZoxHF19TnS2d7h3YAiSzhRxd_8L9oAh7wJHicSM "View from the Kobe Port Tower")

## Privacy & Data Protection

In May 2018, the world drew breath as the European Union implemented the General Directive on Data Protection and released a flood of privacy updates and compliance work into the legal and policy space. Like many multinational bodies, ICANN didn’t escape the GDPR’s scope and quickly ran into problems with their maintenance of the [WHOIS records](https://whois.icann.org/en/about-whois), a method of querying information about who is behind a given domain name.

A WHOIS query reveals information not unlike that of a company or PPSR search in Australia including the name of the registrant, address, telephone number, and email address. This information is contractually required to be accurate as per the agreement between the registry and ICANN. This caused an issue for the registries located in Europe as they were obliged by the GDPR to reduce the information available through WHOIS while also obliged by their contracts with ICANN to maintain all such information.

Immediately following the implementation of the GDPR, ICANN implemented a temporary specification for WHOIS which enabled registries to provide only limited information about their domains while simultaneously starting an [Expedited Policy Development Process](https://community.icann.org/display/EOTSFGRD/EPDP+on+the+Temporary+Specification+for+gTLD+Registration+Data) (EPDP) to sort out the WHOIS and GDPR conundrum going forward.

ICANN64 represented the end of Phase One of the EPDP, wherein the question of what data to provide in the WHOIS was resolved. Phase Two, which deals with how authorised parties can get access to that data, is just starting to get off the ground and will take place over the following year. It’s not to be understated what a mammoth undertaking this is; normally policy development takes place over several years – not the seven months that Phase One of the EPDP had.

It’s important to point out that this relates squarely with the GDPR currently. As far as I know, the scope of the EPDP is limited to such a solution as that which would reduce the legal liability of the registrars under the GDPR. However, the GDPR isn’t the only privacy and data protection law out there, and in Australia at least the [OAIC has raised concerns about WHOIS data in the past](https://www.oaic.gov.au/engage-with-us/submissions/whois-policy-review-for-the-au-domain). As I was there presenting on Data Protection laws in Indonesia and one thing I picked up on while researching the topic was that Indonesia is adopting many data protection measures from the GDPR. As a result, I feel ICANN needs to be more aware of privacy regulations outside the GDPR, lest they run into this whole problem again with another country.

I raised this issue with multiple people throughout the meeting, including a couple of ICANN board members, and got a few encouraging responses. Basically, the focus on the GDPR is one of necessity as it is an imminent threat to WHOIS, but there is a recognised need to develop a comprehensive framework to deal with privacy laws throughout the world as they arise. There hasn’t been much work on this thus far, but it’s heartening that there is some recognition of the issue at the highest level.

<img src="https://raw.githubusercontent.com/ejmann248/blog/master/assets/images/vendingMachine.jpg" height="200" />

## General Internet Governance

If anything, the ICANN meeting opened my eyes to the world of Internet Governance. Alongside ICANN, I heard from and met with people from the [Internet Governance Forum](https://intgovforum.org/multilingual/), the [Asia-Pacific IGF](https://www.aprigf.asia/) and the [Asian Internet Governance Academy](https://www.facebook.com/ap.ig.academy/). I’m keen to get involved with all of these programs and it was particularly interesting to hear that the [Australian Internet Governance Forum](https://www.igf.org.au/) hasn’t been running for the last few years and I’d be interested in seeing what I can do on a local level to advance the awareness of internet governance in Australia and within Swinburne.