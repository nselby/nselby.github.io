---
published: true
layout: default
---
<h1>FreeAgent: Blaming-The-Customer-As-A-Service</h1>
<p><img class="right" width="400px" src="https://nselby.github.io/assets/img/freeagent.png" /></p>

When I used to help run the Fudsec blog, we would highlight people who would use fear, uncertainty and doubt to sell security. Never before have I encountered a company that used FUD to cover up for customer service incompetence and lack of customer support. Then I used FreeAgent. 

We used it for the accounting software for our small company of four people. 

FreeAgent bills itself as ‘online accounting software’ that is ‘your business’s best friend’. I chose it because it had a reasonable UX, and because it allowed two-factor through the Google Authenticator client, something used by lots of other sites. 

When you sign up for the two-factor, it provides you with recovery codes, and warns you of a pain-in-the-ass should you need to log in after losing your two-factor token generator without the recovery codes. 

The Google Authenticator app is a Time-Based One-Time Password algorithm that generates a new, one-time passcode every minute. Now, I am (a) constantly on the road, and (b) don’t even own a printer, so what they were asking me to do as a backup plan was to store these static keys locally, removing all the benefits of two-factor, or two-step, authentication scheme. Most other sites get around this in some kind of automated way. I was to learn that FreeAgent's mysterious CTO doesn't have one of those. 

Here’s something else: lots of people use their smart-phone as a hardware token these days. When using a smartphone, lots of people have to reset them, and when they do, they need to regenerate their keys on Google Authenticator. Other sites I use that have Google Authenticator include GitHub and Gmail, neither of which offered any particular drama when I needed to do this. 

But on FreeAgent, when I sent in an email to support, it was a problem. Oh, wow was it a problem. Actually, just getting an answer was a problem.

<h3>First Contact: 25 January 2017</h3>
On January 25, I wrote to FreeAgent support saying that I had locked myself out. I received the standard “Thank you for getting in touch. We'll get back to you soon, usually within one working day,” email from FreeAgent. 

The next day, I received a message from Stuart Mcewan: 

“Thanks for getting in touch and hopefully I can help. I'm sorry to hear you've had trouble with your mobile phone and no longer able to access your FreeAgent account. As you didn't save the recovery codes somewhere, I'll need to pass you over to our Technical Team who would need to take you through verifying your identity in order to assist further with this. They will be in touch as soon as we can.”

I see. OK. I’ll wait. 

On 27 January I heard nothing. So I wrote back, saying I’d heard nothing.

On 28 January, I heard back from Dave Jones. 

<blockquote>“Apologies for the delay in getting back to you, we're in the midst of tax return season here in the UK, which is why I'm working the weekend shift 😄

“I understand that you're locked out of your FreeAgent account, due to having reset or replaced your phone. From our support history, I see one of your colleagues had the same issue, though since he was a sub-user on the account, we were able to contact you (the account owner) to validate his request. Normally, for dealing with lock-outs on the primary account owner, we compile a set of questions from the data in your account, which you must correctly answer to assert your identity. On this occasion, however, it looks like you're only using a small subset of FreeAgent's functionality, which limits the questions we can pose.

“I'm going to consult with our CTO on the steps we can take to reasonably verify your identity.

“As a security professional, I hope you understand why due diligence is important here. Since you've lost your ability to generate 2 step verification codes, and don't have a copy of your recovery codes, we need to take appropriate measures to protect against potential Social Engineering attacks.”</blockquote>

Now, this might sound all fine and good, but what they have actually done is take, so far, three days to blame me entirely for the problem (which, as I said, from a security standpoint isn’t actually 100% fair but I’ll be happy to take 50% of the blame), and not offer any solution, any estimate of the time necessary to solve the problem, and admit that this is such a flummoxing problem that they need to contact the company Chief Technology Officer in order to suss out how, exactly, to confirm my identity.

<h3>What They Could Have Done</h3>
I’m just going on a limb here:

<ul>
<li>They could telephone me on the number they have in my account</li>
 <li>They could telephone or email some of the other people who access the account and ask them whether the boss is having any issues</li>
 <li>They could text me a one-time code to my mobile phone</li>
<li>I could photograph my driver license and passport and send it to them</li>
 <li>They could ask me some questions about the account that presumably only the account owner would know</li>
</ul>

I’m just spitballing here, but if I can think these things up, surely the ol’ Chief Technology Officer might have a way of thinking up some? 

In any event, I was apparently to understand that “Dave” was busy because of UK Tax Season. Too busy to care about my problem of accessing my customer and accounting information.

<h3>Three Days Later…</h3>
Three days later, I get an email from Dave. It’s about half past noon, and I see this, sent 31 Jan, 17:16 GMT

<p><img width="800px" src="https://nselby.github.io/assets/img/Dave_31_Jan_tried_calling.png" /></p>

So Dave has waited until the <em>very end of his workday</em> to call me, and when he misses me, leaves a voicemail and asks me to set up a time for the next day, at which point he will “convert” the actual time between UK and Eastern Time (what the hell are we doing, sending Pathfinder to Mars? Subtract five, Dave, it’s not calculus) and call me back on the registered number.  

By now, six days have passed, and Dave’s action has necessitated a seventh before we can even converse. I am still not in my account, and the only attempt to actually speak with me personally has been, in my experience, the same sort that you do when you have a bad first date and you call intentionally to get their voicemail.

I write back:

“Are you guys trying to make this harder? I am on the road. In NYC. Why don't you find some challenge questions to ask?  This has taken more than a week.  This is ridiculous. Don't tell me it is because of security. Security includes AVAILABILITY.”

The next reply is astounding. It includes a full-on blaming of me for everything that has transpired, including their monumental customer service failures. When in doubt, blame the customer, I always say:

<p><img width="800px" src="https://nselby.github.io/assets/img/Dave_Reply_2.png" /></p>

Just some observations from this intensely passive-aggressive, yet churlish, email:

<ol>
 <li>He blames the tax season (again - what, has <em>tax season</em> not happened before?);</li>
 <li>He blames the time difference (it is East Coast +5, meaning that when it is 2 pm in Edinburgh, it is 9 am in NY; however Dave didn’t call me until 5:31 pm his time – he expects that Americans don’t know how to tell time, and expects me to feel bad that he “worked late” - Oh, say, Dave: you may have <em>stayed</em> late, mate, but you accomplished no <em>work</em> that I can attest to);</li>
 <li>He tries to confuse me by saying I have asked him to turn off 2-factor without any further checks. Nothing can be further from the truth, it’s just that he hasn’t bothered to make contact with me;</li>
 <li>He blames me again for not holding static codes to open a dynamic system, reducing two factor to single-factor, multiple-credential;</li>
 <li>He implies that I should know better, since this had happened to another of my employees (he’s right, we should have canceled months ago);</li>
 <li>He says all of the above and then tells me that he is not using security as an excuse, but rather, he is simply a bureaucratic oaf working-to-rule, what can you do?;</li>
 <li>He writes all this in a 500-word email, after receiving an email from me (thus understanding that I am now available) rather than calling me back.</li>
</ol> 

My response was rapid fire:
<blockquote>For example, the amount of time it took you to write that long-winded and infuriating response could have, conceivably, been used to CALL ME AGAIN AND GET THIS TAKEN CARE OF, rather than prattling on about time zones, tax season, and contractual mumbo jumbo. All these things are utterly irrelevant to the fact that you have taken DAYS to get a simple provisioning issue handled. Don't try and fob me off and tell me that you are working to rule, Dave, FIX MY PROBLEM</blockquote>

<h3>They Have A Plan</h3>
The next day, February 1, I receive this note from Dave:
“Please provide me with the details of any invoices and expenses that you've entered into FreeAgent. Details should include, but not be limited to, dates, amounts and associated contacts and projects.”

So, after all his posturing about “security” and “easily spoofable” information, the information that FreeAgent will accept – instead of the more bulletproof examples I postulated above – are copies of the invoices I have sent in the past to clients through unencrypted email. 

Gosh, they <em>are</em> living up to the letter of that terms of service agreement, aren’t they?

Of course, since I am on the road, still, I am unable to even do that. But – wuh-heh-hey! – we’re in business, right? 

On February 4, I send them a bunch of invoice information, cut-and-pasted from an employee’s account that still had access to the invoices. 

Randomly, really.

Then, on February 6, I heard from The FreeAgent Fairy! It gave me a list of outstanding invoices that had yet to be paid, called, cleverly, The Monday Motivator, asking me cheekily, “What's on the agenda for this week?” and threatening, “See you next Monday!” 

Yet no support response had arrived.

I wrote back to support, “Really want me motivated? Please help me get back into my account that has been open ticketed for TWO WEEKS.”

<h3>Second Response From Support: 6 February 2017</h3>
Debbie writes back, “Thank you for your email today. I can see that our technical team are currently working on this for you and will be back in touch shortly. Thank you for your patience while we sort the login issue for you.” 

Golly! That is super friendly. They’re working on this. For me. I responded, 

“To paraphrase Hobson, I await their next syllable with utmost eagerness.”

“Thank you for getting in touch. We'll get back to you soon, usually within one working day,” said FreeAgent.

Finally, also on February 6, I get an email from Peter Singh:

<blockquote>“Hi Nick, Peter here from Support Engineering at FreeAgent again - many thanks for sending us through the information that Dave had asked for. I've now cross referenced the information given against that which is in your account, and I'm happy that it is all accurate.”</blockquote>

Golly, I’m thrilled. 

Two weeks to turn-off two-factor so I can log back in. 

I have more than 10 accounts in my Google Authenticator. When I replaced my phone, this was the only one that had an issue being replaced. All the others automatically replaced the key, some by sending me through to a QR code while I was logged in, some by automatically sending a text to the registered number they had on file. 

None made me deal with a sniffy, passive-aggressive little turd in Edinburgh. 

<h3>My Reply to Them:</h3>
I sent them this note afterwards. Was the last line ill-advised? Possibly. However, after what they’d put me through to access my data, I was angry. 

“I am now going to explain something I hope your CEO/MD, head of marketing and CSO see. You made me wait more than two weeks to gain access to this system. Do you know what I learned in that time? 

“That I can. 

“I can live without you people forever. You gave me excuses ("it's tax season"). You blamed me ("when you signed up you were told..."). You wrote long emails rather than taking the time to help me. And even after I sent you the documentation (available, I might add, to my CLIENTS as well as to me, and in no way documentary proof of anything), you waited until almost 10 in the morning LOCAL time, despite it being mid-afternoon your time, to get me sorted - and then it was only after I wrote in to complain. This tells me that you care not a whit about my problems.

“As I mentioned earlier, security is confidentiality, integrity and availability. My system was unavailable to me for more than two weeks, rendering it insecure. 

“Your pleas of doing things in the name of security were meaningless, because your continued delays in getting me what I, the customer, needed, continued the unavailability. Here's something of mine you had: my mobile number. You could have texted me a code. You could have asked me to send in a photo of my driving license. Or my birth certificate. You might have asked another of my colleagues whether I was actually having the difficulty I claimed. 

“Instead, you did nothing. 

“So let me tell you assholes something: you've lost my respect. You've lost my business. Worse than that, I will tell each and every person I know just how much you suck. I know quite a few people. I intend to go quite public with this tale. I will blog about it, I will podcast about it. I think you can expect the tail of this tale to be long. 

“Fuck each and every one of you to death.”

After that, we got our data ready and moved it to another service. We'd already finished and had not got round to deleting the account.

<h3>Their Reply To Me: You're Fired</h3>
Then, Lo! Another email this morning. 

They’re firing me as a customer (thank Heavens for small gifts):

<blockquote>Dear Nick
I refer to your email conversation reference number 259955 with David Jones.

While we welcome constructive feedback to help us improve our services, we will not, under any circumstances, tolerate anyone swearing at our staff and using abusive language.

In accordance with our terms and conditions we reserve the right to cancel a customer’s account at one month’s notice.
Please be advised therefore that unless we receive a full written apology from you in the interim for the unacceptable language you used in your responses to David, we will cancel your account on Tuesday 14th March 2017. This cancellation will be irreversible.

We will refund the unused portion of your subscription to you at this point.

Before Tuesday 14th March 2017 please make sure that you export any data you had in the account, by choosing Export All Data from the Settings page which will export your data to Excel, which you can retrieve from the Files area in FreeAgent.

If you have uploaded any files into FreeAgent, either in the Files area or as attachments to transactions, you will need to download these separately from the export to Excel.

You should also save copies of your invoices as .pdfs, and save copies of your profit and loss accounts, balance sheets and trial balances for each year.  To find the latter, go to Accounting > Reports.

Once we cancel your account you will not be able to access any of your data again, so I say once again, please make sure you do this before 14th March.

To avoid cancellation of your account we would require you to apologise fully and unreservedly to David in writing.
Yours sincerely

Emily Coltman FCA
Chief Accountant</blockquote>

<em>Yours sincerely!</em> What a card!

To which I replied,

“Dear Emily,
Ha ha ha ha ha ha ha ha ha ha. Delete my data. I want it off your system. Every single datum. Gone. Send me an attestation of destruction along with a full refund for every single day remaining on my subscription.

And they replied,

<p><img width="500px" src="https://nselby.github.io/assets/img/thanks.png" /></p>


