## Usable Security Blog
## June 11, 2020
Zero Trust Networks 

Usable Security – Case Study 

Section 1: Trust  

Trust is not only defined as the absence of risk and uncertainty, but is also defined as a complex human response to situations that contain this risk and uncertainty. To establish trust there are a few requirements that must be fulfilled. The first requirement is vulnerability. When people are vulnerable, trust inherently exists. When establishing trust both parties are vulnerable to the betrayal of the other party. The second requirement to establish trust is optimism. In a trusting relationship there needs to be some level of optimism that the other party will have a motive for action on their behalf. The third and last requirement needed to establish trust is competency which is the assumption that individuals will possess the relevant skills or ability needed to perform an action. 1 

The two general types of trust are (human-to-human) interpersonal trust and (human-to-system) system trust. An interpersonal trust relationship develops over a period of time when an expectation of trustworthy behavior is fulfilled between two individuals. However, it is important to note that interpersonal trust relationships are highly dependent on the specific situations in different social interactions. A system trust relationship on the other hand does not develop over time or depend heavily on different social interactions. A system trust relationship contains a complex layered arrangement of systems and networks. These arrangements carry different layers of trust. This can be seen in protocols that often presume there is a reliable and trustworthy relationship between these networks.2 

There are two requirements needed to establish trust in a network environment. The first requirement is secure end-to-end communication. The second requirement is that security is created with no expense to survivability. Security should not be confused with privacy. Security enables the control of digital information while privacy requires that an individual be able to control their personal digital information.  Survivability is the idea that any network should be able to degrade gracefully rather than failing critically. Survivability can be established with distribution and graceful degradation. Graceful degradation means that when one section or device of a network fails this does not affect the rest of the network. The actions of one person does not alter the access of others. 3 

The three-dimension model of trust in a system or network is based on risks rather than user perception of risk and require privacy, security, and reliability. Privacy is based around vulnerability and optimism. Security must be based around motivation and competence. While reliability is there result of the belief in integrity and competency of a party. Trust in a network is mostly influenced by the humans, organizations and governments that control them rather than the network itself. 4 

 

Section 2: Issues with trust in networks 

Now with an understanding of trust and how it relates to network environments, we can examine the issues that trust brings with it to networks. 

One of the most important aspects of a trust relationship are the origins of the commitment and its context.5 Often to complete some general “task”, there usually must be some trust agreement between the parties involved but this can be easily undermined when the ends of the agreement are just for completing said task. For example, in the event of a new hire, the new employee will likely agree to any password policy just because they want the job, so they begin a trust relationship without necessarily fulfilling the original agreement. In some situations, no matter how the original commitment is formed, there is no ability to build trust.  

Overreliance on assurances is another large issue with trust.6 Assurances can range from contract or user agreements to social norms. This brings problems when we blindly accept people’s trust based on social agreements or contracts because we see only the agreements instead of what’s happening in reality. The social contract view provides us with an example of a male employer who is “extra” nice to female co-workers to make it seem like he's treating employees equally.7 Though this still results in sexist behavior and he fails to build trust because the employer is trying to take advantage of our social contract.  

A third problem surrounding trust is inferring trust. Inferred trust can be both implicit and explicit (signals/cues vs. ratings/reviews) although in either case they can lead to deception, exploitation & misinterpretation. Any of these inferred results can be extremely damaging in a network setting since it will turn into a significant vulnerability that an attacker could exploit. If you were to assume every review on Amazon was a legitimate user, you could very easily be led into a disappointing purchase of something that you had inferred would be something else. 

The last issue is the idea of an “All-or-Nothing" trust systems. In traditional network environments it is very common to design the network to have a secure perimeter around your assets. The idea of a castle surrounded by a moat. This has the inevitable failing of once that perimeter is broken all the assets are then accessible. This clearly causes huge security risk in that in the event your network gets comprised, everything gets comprised.  

All these issues present massive vulnerabilities and with constantly evolving infrastructure, we see organization re-thinking their trust models. This is the basis to why there is a push to remove trust completely from corporate environments. 

 

Section 3: Examination of Zero Trust principles and design application 

 

Microsoft principles of Zero Trust: 

Verify explicitly. Always authenticate and authorize based on all available data points, 

including user identity, location, device health, service or workload, data classification, 

and anomalies. 

 

Use least privileged access. Limit user access with Just In Time and Just Enough 

Access (JIT/JEA), risk based adaptive polices, and data protection to protect both data 

and productivity. 

 

Assume breach. Minimize blast radius for breaches and prevent lateral movement by 

segmenting access by network, user, devices, and application awareness. Verify all sessions 

are encrypted end to end. Use analytics to get visibility, drive threat detection, and 

improve defenses. 

Microsoft tools to drive implementation: 

Strong authentication. Ensure strong multi factor authentication and session risk detection as 

the backbone of your access strategy to minimize the risk of identity compromise. 

 

Policy based adaptive access. Define acceptable access policies for your resources and 

enforce them with a consistent security policy engine that provides both governance and 

insight into variances. 

 

Micro segmentation. Move beyond simple centralized network-based perimeter to 

comprehensive and distributed segmentation using software defined micro perimeters. 

 

Automation. Invest in automated alerting and remediation to reduce your mean time to 

respond (MTTR) to attacks. 

 

Intelligence and AI. Utilize cloud intelligence and all available signals to detect and respond to 

access anomalies in real time. 

 

Data classification and protection. Discover, classify, protect, and monitor sensitive data to 

minimize exposure from malicious or accidental exfiltration. 

 

WWU Zero Trust Principles: 

Monitoring must be present throughout the network. 

Constraining done by the policy agent must be dynamic and strict. 

Direct trust relationships must be built between users and systems and the Trust Engine. 

Trust cannot be inferred through any system or relationship. 

The inner workings of the control plane must be opaque to the end-user. 

The control plane should have redundancy with fall back controls as well as scalability. 

-design 

 

Section 4: Case Studies of Zero Trust: Google, Microsoft, and WWU Zero Trust 

Zero Trust is a relatively new concept for protecting and securing networks, and as such large corporations with a wide attack surface are the primary developers of standards and best practices. The Zero Trust ideology was first introduced by Google under the name BeyondCorp which was a response to the Advanced Persistent Threat (APT) attack by China in 2009 codenamed Operation Aurora.8 Unlike the traditional perimeter security model, BeyondCorp dispels the notion of network segmentation as the primary mechanism for protecting sensitive resources. Instead, all applications are deployed to the public Internet, accessible through a user and device-centric authentication and authorization workflow.9  

There are several novel systems Google employs for this authentication and authorization, namely the access proxy and the access control engine. Gaining access to a resource on the network begins with the access proxy which incorporates several well-established security solutions like Single-Sign On (SSO) and device certificates. When the user attempts to connect to the BeyondCorp network the access proxy negotiates the device certificate with a database of known managed device, then it will redirect the user to the SSO system. Once the device certificate is found and the user is properly authenticated the access control engine is the next step in the process. The access control engine confirms the following information: 

The user is in the correct group to access the resource. 

The user has a sufficient trust level. 

The device is managed and in good standing. 

The device has a sufficient trust level.  

If all these checks pass then the user and device can access the resource, if any single one fails the request to access the resource is denied.10 

Google BeyondCorp’s transparency has allowed many organizations to capitalize on this new ideology of security, notably Microsoft who has published their own papers detailing their principles of Zero Trust. Microsoft keeps their specific implementation of Zero Trust opaque and instead opts to give out more general guidelines, standards and principles. Microsoft also offers a maturity model so that organizations can determine their own level of adoption of the Zero Trust ideology. The first level is a Traditional network security architecture consisting of: 

On-premises identities with static rules and some SSO. 

Limited visibility into devices, cloud environments and logins. 

A flat network infrastructure.  

The second level is Advanced which involves the following: 

Hybrid identities are formed from multiple data sources fine-tuned access policies for access. 

Devices are managed and registered in a database. 

Networks are segmented and cloud environments are monitored. 

User behavior analysis is implemented to proactively identify threats. 

The third level is the Optimal implementation which includes: 

Cloud identities with analytics and dynamic access to apps, networks and data. 

Data access decisions governed by policy engine with encryption and tracking. 

Trust has been removed from the network entirely with micro-perimeters and segmentation as well as encryption. 

Automatic threat detection and response are implemented.11

As shown above, Microsoft chooses to focus more heavily on policy to implement Zero Trust and forgoes the idea of an access control engine that Google implements  

 

Bibliography 

[1] McLeod, Carolyn, "Trust", The Stanford Encyclopedia of Philosophy (Fall 2015 Edition), Edward N. Zalta (ed.), URL = <https://plato.stanford.edu/archives/fall2015/entries/trust/>. 

[2] Cheshire, Coye. (2011). Online Trust, Trustworthiness, or Assurance?. Daedalus. 140. 49-58. 10.1162/DAED_a_00114. 

[3] Camp, L. Jean, Design for Trust. TRUST, REPUTATION AND SECURITY: THEORIES AND PRACTICE, Rino Falcone, ed., Springer-Verlang (Berlin), 2003. Available at SSRN: https://ssrn.com/abstract=627610 

[4] Gilman, E., & Barth, D. (2017). Zero trust networks: building secure systems in untrusted networks. Sebastopol, CA: OReilly Media.  

[5] Zero Trust Maturity Model. (n.d.). Retrieved June 10, 2020, from https://go.microsoft.com/fwlink/p/?LinkID=2109181&clcid=0x409&culture=en-us&country=US 

[6] Ward, R., & Beyer, B. (2014). BeyondCorp: A New Approach to Enterprise Security. Retrieved June 10, 2020, from https://storage.googleapis.com/pub-tools-public-publication-data/pdf/43231.pdf 

[7] Dinkelman, S., Stuifbergen, J., Traner, J., & Anderson, S. (2020, June 3). WWU Zero Trust Networks. Retrieved June 10, 2020, from https://wwuzerotrust.com/Documentation/ 

[8] Baier, A. C., 1986. “Trust and Antitrust,” Ethics, 96: 231–260.  

[9] –––, 1991. “Trust and Its Vulnerabilities” and “Sustaining Trust,” Tanner Lectures on Human Values, Volume 13, Salt Lake City: University of Utah Press. 

[10] –––, 1995. Moral Prejudices: Essays on Ethics, Cambridge, MA: Harvard University Press. 

[11] –––, 2004. “Demoralization, Trust, and the Virtues,” in Calhoun (ed.) 2004. 

[12] Run Zero Trust Security Like Google. (2018). Retrieved June 10, 2020, from https://www.beyondcorp.com/ 

## May 25, 2020

Data Void
There are positives and negatives to everything. Youtuber sponsored videos. Racoon earbud reviews are terrible, yet your favorite creator swears up and down that they are amazing.I do not feel qualified to have this discussion, because I have no idea how a search engine works underneath the hood.  I don’t know the best ways to apply SEO to a website. Google may serve users incorrect information or “lead users down dark rabbit holes”, but I think google as a whole works pretty well! If we went back to the dark ages, they would burn people at the stake for being a witch. The spread of misinformation will always exist, I don’t see a perfect scenario, because technologies always leads back to the user, which are people. And people act in self-interest.
 I think there should be pressure on companies like google to continue perfecting their search algorithms, but somewhere people will find some information that they will read. They will have to decide for themselves if it is true, or perform more research. In some instances like the Sutherland springs Texas situation, it is hard to know what information is correct. 
Even if there was a perfect search engine that could funnel out all mis information and silence groups behind the “crisis actors”, Would that be encroaching the right to free speech? 

Data craft:
Meta data is important for defining anything on large platforms with lots of data. Brian Babin twitter account example. 3 of the accounts are almost undistinguishable, there are  fakes, and just by looking at the meta data it is to hard to tell the difference. 

Government accounts inactive for 6 months will be closed. They are then open for resubmittion. Example showed that they got hold of @USEmbassyRiyadh account. 
This article showed how meta data is great for classifying user posts, but can be abused. 
This is hard to relate to as I don’t have a twitter or Instagram. I don’t use Facebook very much if at all. I think the example of twitter accounts being compromised, and fake accounts being mixed in with real ones is issue that twitter needs to fix, as people rely on twitter for news  and credible information. Other platforms may have pseudonymity, such as YouTube. A YouTube account has its reputation biased on its content. A twitter account does not provide any pseudonymity, as the account is based on a real person.
 Meta data is involved with literally any social platform. The concept of meta data is personal data is the definition of the entire big data market and targeted advertisements. Which this stems a much larger conversation if target adds should even exists. 


## May 19, 2020

Biometrics dehumanizes people. Essentially reduces a complex human to data points. Essentially this is authentication. Can we rely on biometric data? As we become more reliant on technology, they technology may be flawed, therefore our decisions are flawed. Can biometric tech be used as an extra step in our current ways of identification. Resulting in a more streamlined process. The argument that biometrics dehumanize people is interesting to me. I personally don’t find it an issue if me as a person is summed up into data points. I am not saying I agree with widespread use of biometric identification. In a perfect world if biometric data was used responsibly and had no technical flaws, I don’t have an issue being summed up into data points. I don’t that to be my identity, I don’t think of passwords as my identity. I don’t think of my social security number as my identity. I am interested 

What about non collision hashes for biometric data? Keep the positives of the authentication via Biometric tech while maintaining anonymity. I think if there was an opt in service where biometric data were to be used, it should maintain a form of anonymity. Again I am maintaining that there should be a process for identity that is paired with biometrics, as we cant solely make our decisions based on a flawed technology.

Immigration in South America seems extremely messed up compared to the united states. Using ID cards to separate the population based on the tone of their skin. Sometimes people would get reclassified. This had insane consequences as it heavily changed people’s lives. The South American government used an weird classification method. It was first used to classify animals. Basically, different genres. This was a very old approach, and they applied it to people. I cannot believe that they didn’t allow different classifications of people to marry. Applying race based on the color of a persons skin isn’t even scientifically accurate. The article showed an example of a boxer being re classified from white to a different classification right before a big match. He lost everything right before the match. Was the cauterization used to oppress people? In relation to the US census, I think that it is used for demographic understanding. I think the main point of this article is that we need to be careful of placing labels on people. When you put labels on people, it can be dehumanizing. Another key point of that this article said was that applying labels to groups of people may disenfranchise other groups.  

## May 12, 2020
This week reading was about security tools and encryption. How everyday persons not involved deeply in technology and security use security tools in their lives. People do not know the interquel details of how encryption works, and nor should they. The studies in the readings indicated that most people didn’t value security, and just widely accepted that everyone worked, and designers spent just as much time as the functionality of their application as they did on security. I find this reading heavily relates to the ethnography in technology. The use of technology between cultures and countries are not the same. They are viewed differently, and an actor theory network map might not have the same results in different cultures. 

Encryption is extremely important tool, as it insures privacy. In the readings, users were not sure the basics of encryption and they use it every day. I think the example of score cards rating the applications use and quality of the encryption is a great idea to help everyday consumers. Consumers should not have to read the intricate details of how key exchanges work. The score should be expanded to incorporate a set of security tests that the application should withstand. This could be a governing body attached to application stores like apple store or google store. It would be impossible and extremely costly to perform tests on all applications on the store, and it would also hurt the small developers. However the security score cards could be an amazing idea for the popular applications that millions of people use. If an application reaches a certain mass of users, they will have to subject their application to a security test. 

Billions of people have driven cars, but all of them do not know the mechanical components of their cars. The argument that consumers knowing the details of encryption is pointless. Also, there is a point that is brought up in the reading that people are just lazy and they don’t care. If the applications function like they need it to, most people are not going to dig deep into its security components. Even if the application has a very low security score (on our imaginary security scoring system for applications) they may not want to find a new application and learn how to use it. Given that point, I think the most important solution is to prove to consumers that their security has value. 


### April 29, 2020
This weeks readings asks the question, what will the internet be like in the future, and who will shape it. ARPANET was the beginning of the internet, connecting computer systems together around the world, and it was “pure and simple”. Now the scope of todays internet is massive. One big discussion is the fact that billion dollar companies are gaining control of the internet. Not control of the internet like banning where you can and cant navigate to using rules, but more of a monopoly. Many believe that these companies have too much control and are abusing their power. One idea was creating a democratic internet, where large companies did not have so much power. Where amazon was not the one stop shop, and customers would go to other websites as well to purchase their items. Disney now has a mind-blowingly amount of companies. Just look at this diagram!

<img src="https://storage.googleapis.com/titlemax-media/1c8ace8f-every-company-disney-owns-13_pageversion-lg.jpg" alt="low" class="inline"/>

The internet is where it is today because of consumerism. I think harsh regulation is not the answer. If consumers use a website or service because they enjoy the platform, users should not be forced to navigate elsewhere. Most companies exist because they invented a service or solved a problem. Competition breeds innovation. I do not think it is right for large companies to continually buy out smaller startups, as they no longer have to compete. I think it is important for the government or a controlling body to steer the internet in a way that’s best for the masses. Apply regulation and fines for privacy and security. Enforce a right to compete standard that eliminates mass buyouts of companies. 

It is important to have a controlling body though. As the world of internet of things devices are Everly increasing, protocol standards and security regulations are extremely important. 

### April,20, 2020
Ethnography, the study of interactions and reactions of different social cultures. Researchers need to gather observations, interviews, and documentary data for detailed accounts of different social phenomena. When companies are close to the final release of a product, they try to have unbiased test groups come in to use their product. Their reactions are important to judge how close the product is for release. However, I never have thought about Ethnography in relation to technology. How one service or application can work great in the united states, but the success my not work in other countries. It is helpful when releasing products and services in different countries. I see this being an important stage when developing a hacker methodology map, as discussed in my previous post. Paul Dourish brings up the use of Ethnography and points out that it is hard to pinpoint where the reactions come from. 

You cant just be a “tape recorder”, a ethnographer must go more in depth. Subjectivity is an important aspect while being an ethnographer. If data is just collected, it is too hard to correctly identify what stemmed from where. It is noted that engineers tend to leave subjectivity out of ethnography.  

Many tech companies today employ lots of ethnographers, as they want to perform product research, and find new areas of markets. As a future security professional, I want to take the techniques of a ethnographer and apply it to usable security. A way to judge new security policies implemented in the work place. It may already be apparent if there is a poor policy implemented in the workplace as many employees will complain. However, ethnography can uncover problems that a design can fix.

Dourish, Paul. “Implications for Design.” CHI, 2006, pp. 541-550.

### April,17, 2020
This week, we read an academic paper called Norman DesignX sociotechnical systems. This paper showed how designers now face the challenge of designing complex sociotechnical systems. It explains that designers need to be a part of the implementation stage. This is because not everyone processes and understands the same way that others do. This paper also explained the concept of release products using different methodologies. The hacker methodology means that the designer should know the entirety of their products impact on everyone and everything before releasing the final product. In a perfect world, I may agree with that methodology. However, in many times over the engineer or designer will release a product that was used entirely in a different way than it was intended for. The keyword being intended. No one can accurately foresee the use case of their product. Even if they could, designing their product around every possible use case will result in something that is bad at everything. For example, if GM just made one type of vehicle. If GM tried to make a car that is comfortable but sporty, small and economical, Burly with a lot of torque for pulling, Low to the ground for handling while being able to go off road. That will result in one really bad vehicle, but it takes into account every possible use case that someone might use it for. That just wont work. Therefore, GM makes economical cars, comfy cars, sporty cars, trucks, etc. Designing your product needs to be for a specific use case. 

One interesting topic that was brought up, was the fact that people tend to engineer systems and services by breaking them down into components. Components that are usually responsible for 1 process, and usually don’t have more than a linear relation with the other components of the system. Because of this, ideas or possible designs that don’t meet most peoples thinking process are thrown out. I have a hard time materializing that statement. I don’t know how to quantify which ideas were amazing but had to be thrown out because it didn’t fit our way of thinking. The issue with this argument is for something to be widely used and adopted, it needs to be understood by many on how it operates. Think of vehicles or open source programs, if only a few people knew how to work on cars because they were so complex, no one would have them. If only a few people could work on a open source program, that program wouldn’t exist or it would be very barebones. Complex products and services need to be made of components; they need to be modular so everyone can understand. Systems also must be continuously updated to keep up with new technology, or it will be unusable. 

Norman, D. A., & Stappers, P. J. (2015). DesignX: Complex SociotechnicalSystems. She Ji, 83–107. Retrieved from http://www.journals.elsevier.com/she-ji-the-journal-of-design-economics-and-innovation

