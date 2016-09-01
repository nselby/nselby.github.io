---
published: true
layout: default
---
<h1>By ‘Secure’, We Didn’t Mean...</h1>
<p><img class="right" width="450px" src="http://resources.infosecinstitute.com/wp-content/uploads/it-security-analyst.jpg" /></p>


<p>During a response to a security incident at a financial institution, I came across a very bad situation: a managed security service provider (MSSP) that had managed to put their sensors in the wrong place, ensuring that the customer got neither security or service.  Now, anyone can misplace a box. What was surprising to me was the period of time it took to discover the misplacement.</p>

<p>At first, the issue was just a little funny: when they claimed that they had some issues on their network that sounded like rather classic symptoms of a botnet, I asked what they had for visibility. They told me that their provider had put a box of sensors on their network so that they could continually monitor logs and traffic. Great!</p>

<p>But when they went downstairs to examine it, they immediately discovered that the MSSP had instructed them to place it on the wrong side of the firewall and it wasn't seeing any of the traffic it was supposed to be looking at.</p>

<p>The box, the client told me, had been installed <em>three years earlier</em>. And it wasn't the MSSP that discovered it, but rather the customer, and only after their hair was on fire.</p>

<p>This meant that, for the past three years, the box would have been seeing vastly less traffic than was described to the MSSP when they sold the product, and what traffic the MSSP did see would be at a substantially lower volume than expected, and missing some key traffic types, such as DNS requests and logs.</p>

<p>Which would, it would seem, mean that this MSSP both charged the customer and didn’t look at the actual traffic. For “security monitoring,” then, the reports must have been wicked easy: “Y’all look <em>great</em>!”</p>

<p>Hang on a minute. Doesn’t that “Security Triad” thingy talk about this? Under, say, “<em>Availability</em>”? The financial institution told the MSSP it would be monitoring, say, 250 endpoints and 125 servers. Because of the placement of the box, the MSSP saw the traffic of, say, five endpoints, and intermittently at best... Wouldn’t that, you know, in and of itself, speak to a security event if only because of that “Security Triad” thingy?</p>

<p>No matter. Let’s deal with that later. Move the box, put it where it should have been and let’s see what we can get. Except we cannot see anything because the box doesn’t have a customer portal that allows real-time viewing. Just reporting. So we need to call the MSSP. </p>

<p>After ten minutes on hold we get someone who sounds completely incapable of answering the question we have. The question is this: “You are monitoring our network. We have had a security incident. We are trying to see if there is an active botnet on our network. Do you see any beaconing or other behavior that would indicate this?“</p>

<p>After an hour of being transferred to people, the person who understood how the box worked told us all the reasons he should not look at his box to answer the question. “You have a monitoring account,” he said, “What you are describing now sounds like an incident response. I would be happy to get our IR team on the line for you...”</p>

<p>My crazy friend Tim was always broke and under investigation, and he used to do an impersonation of an arrogant banker telling him why he couldn’t take any money out. “You see, sir,” the snooty manager would tell Tim, “You have what we call a, “<em>You-can’t-have-any-of-your-money-account</em>,” and what that means is that you can’t have any of your money.”

<p>The MSSP guy was sounding like Tim’s branch manager.</p>

<p>He was interrupted by the CIO of the financial institution I was with, whom I shall call, “Dave”. Dave had taken over the operations about a month before, and inherited all these relationships and all this equipment. “Listen,” Dave said, “I got an incident response crew here. They are good. They are here in some ways because the idiots who bought your services didn’t check to see that your product was actually installed (which it wasn’t) and working (which it wasn’t) and you took advantage of them and here we are. Just tell me the answer to the question: We are trying to see if there is an active botnet on our network. Do you see any beaconing or other behavior that would indicate this?”</p>

<p>After three or four more attempts to not answer, he finally began looking at the box, and calling out different anomalous things that he saw. We worked along with him. Then, out of nowhere, having told us almost nothing, he said these words:</p>

<p>“OK, so I am sorry, but I have a conference call that I have to be on at the top of the hour. I’m going to have to go.”</p>

<p>“Wait,” said the CIO, “Are you fuckin’ serious?”</p>

<p>“Yes, I am sorry but I have a call I must be on.”</p>

<p>“Are you fucking kidding me?” said the CIO, “You guys drop the ball, it takes an hour to get nothing and you’re leaving?”</p>

<p>“Well, sir, it wasn’t ‘nothing’” said the call agent. “I gave you more service than you are contracted for...”</p>

<p>At that point, people on my end of the conversation started being rude. </p>

<p>What I am trying to figure out is how it is possible that this company could have been so taken advantage of by a well-known MSSP. Its propaganda refers to events flying through your network, and the need for experts to review your data and give you in-depth analysis. It speaks of on-demand reporting from a client dashboard, on which colorful yet incisive metrics as to your true state can be revealed.</p>

<p>So something must have gone really wrong? The first two of their certified security analysts sounded as competent and helpful as the folks you get to speak with when you call AT&amp;T to complain that your bill is for too much money. And while the last guy sounded as if he understood what he was doing, it was apparent that what he was doing was not what the customer felt they’d paid for. </p>

<p>I’ve been in the business quite a long time. In my mind, this was the single worst example of security customer service I have ever witnessed.  </p>

<p>Here's one possibility we discussed on the <a href="https://secure-hwcdn.libsyn.com/p/6/6/c/66cbce510556c443/SFS_Podcast_-_Episode_184.mp3?c_id=12605697&expiration=1472522109&hwt=cb4bbfd345a75a9c436ad9a00253e710" target="_blank">Southern Fried Security Podcast</a> tonight: The MSSP could have told the previous team that they weren't seeing the alerts or the traffic, and that team could have blown them off. Sure, that could have happened. Is it incumbent upon the MSSP to review this and try again every year at contract signing? I say that it is.</p> 

<p>So what can we do? We can tell people the truth. We can make it so that even commoditized security services are performed with integrity, and with pride. We can make sure that whenever we sign contracts with people, we live up to their letter and their spirit. </p>

<p>Because this customer is seriously angry. They feel that they were ripped off, and left holding the bag. In my professional opinion, they are not wrong. I saw the moment at which they realized that their expectations as to what type and level of service they had subscribed to ultimately didn't match the service they actually received. It was a bad moment to watch. I've seen this moment a lot in the world of cyber security in the private sector and as a police officer investigating cyber crimes. The customer feels betrayed. They feel tricked. They feel ripped off by those who took their money in exchange for a promise to be there for them.</p>


<p>Is it possible they misunderstood what they were buying for somewhere around $4,000 a quarter? Sure, we professionals understand (the question, 'What did you expect for $16,000 a year?' pops immediately to mind). So take a moment to re-consider the impact of the breathless marketing prose - which, let's face it, isn't exactly out of the ordinary in terms of the words or the sense of promises being made by someone selling managed security services.</p>

<p>It speaks of security experts, standing by to analyze your logs and alerts, 24x7x365. It speaks of locating malicious traffic, and digging through piles of data to find the threats that can shut down your business. And it talks of rapidly providing you with in-depth analysis, inexpensively. </p>

<p>Now, in my opinion, a reasonable person might believe that this meant that, in exchange for their money, they would be getting a team of certified security analysts to compile and sift through their network data, 24 hours a day, hunting for and capturing evil threats that might disrupt their business. </p>

<p>I think that security professionals should help customers review these kinds of contracts. I think we should make it easier for customers to understand what they should expect. I think we owe it to our customers to provide some kind of contract review, some Service-Level-Agreement coaching as part of larger security gigs, so that they don't get snookered. Sure, <em>caveat emptor</em> holds true. But every time we complain that people don't care about security, or when we comment that dumb users and dumb customers are behind breaches, let's ask ourselves whether we as an industry are earning the trust of our customers, those who we serve.</p>

<p>I sure hope we are. </p>


