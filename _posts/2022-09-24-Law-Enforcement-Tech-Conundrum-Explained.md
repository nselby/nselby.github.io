---
published: true
layout: default
title: Law Enforcement Tech Conundrum Explained
---
  

Recently I had to check whether a particular Colt .38 revolver had been stolen. I was checking on the world's stupidest law enforcement Records Management System. So, I entered the serial number, the make (Colt), model (Detective Special), caliber (.38 Special). I immediately was presented with a festival of errors (38 SPEC not .38 Special, etc). OK, so I solved the errors through more trial and error - entering it again, getting more errors, entering it again, getting more errors, and then finally, the query was accepted!

Uh oh. The gun was stolen! 

Wait wait. I read more closely the result. Yeah, the serial number is right. But the gun listed as stolen was a Charter Arms .44 Bulldog, not a Colt .38 Special Detective Special. 

OK, try again... 

Error. Literally five tries later I am awarded, magnanimously, with a screen of the actual gun I was running. No hits. 

As a technology user who has once visited the Travelocity website, I have some questions: 

* How could entering the S/N and manufacturer name of a gun not be sufficient for 99.9% of queries? 
* How could entering be so difficult and manual? 
* How could I enter "38" and get a result for a .44? 
* Come to think of it, how could I enter COLT as a manufacturer and get a result for a Charter Arms gun?
* Etc.

The answers are that the product was made by non-cop, sub-standard, subcontracted, non-native-English speaker developers who are working in deprecated languages, writing crappy code that is not user-tested, to solve problems none of the developers understand. 

To them, my problems were data entry issues. 

To cops, it's a "stupid" issue. 

But the chief is happy. The system "works" in the sense that he can find what he needs when he needs to. The price is right. The cops using it for a long time have developed hundreds of workarounds for the stupidity of the system, so they can function more or less "efficiently". They hate their user experience, but the work gets done. 

All that you just read is a perfect encapsulation of the state of law enforcement technology. 

Recently on Twitter someone asked why paperwork could not be made easier for cops. 

### Five Reasons LE Tech Is Hard

The problems are manifold. 

**First**, every cop hates paperwork but every cop knows that paperwork is the thing that saves your, well, bacon. There's negative incentive to reduce that which covers yer bum.... 

**Second**, we are terrible at buying tech. Cops try to avoid it because it is scary and new and makes them feel uniquely not in charge, which they hate. So they mock it, and learn only that which is required (this also covers butts-if you get good at it, they make you do it more)  

**Third**, vendors of tech know, avg incumbency of a piece of LE tech is ~17 years: the pain of owning must finally overcome the pain of not having a new thing. Then it's an emergency! Decisions get made based on sales promises and fairy dust, not solid tech choices. See "Second".  

**Fourth**, cops/chiefs are suspicious of automation esp. in report writing. It's incumbent on us to write great[[1](#footnote_1)] reports, so automation introduces the specter of automated errors and blown cases. Many cops (ahem) keep boilerplate in a word doc on their computer, unofficially.  

**Fifth**, vendors of LE tech, cognizant of that 17-year incumbency, do everything in their power to limit integration of their tech with that of other companies - even totally non-competitive ones. At best this is to provide a revenue stream of prof. services for integration, but at worst it is to frustrate the agency into thinking it is just too hard to integrate anything, so they stop trying and simply pay their current vendor for new features, which are made crappily, implemented poorly, and generally suck in every possible way... 

As an example: you're in a patrol car and see a Chevy Malibu ahead of you and radar says it is speeding. You want to run the plate but to do so requires the LP *and vehicle description (whyohwhyohwhy?!), so you type "C...H...E..." and the autocomplete kicks in with "CHECKER"... 

Why? Because the vendor is a lazy sod with no LE experience and they found or scraped a list of car makes and posted them alphabetically into the system, and NO ONE THOUGHT TO FIELD TEST THIS. The only cops in the company are in sales, and they only care about SALES... 

In 10 years of driving around in a police car I never once pulled over a Baldwin-Mercury, Baldwin-Motion, Beck, Bentley, or Bugatti - but I sure did pull over lots of Buicks.

Had the cops in the company consulted on this; had user-acceptance testing been conducted in the car, with company product managers watching users actually use the product; then they would have made TWO lists. The first autocomplete list would have ONLY the top brands of cars by ownership - Chevy, Ford, Toyota, Honda, etc. If the car being searched doesn't appear in that list, then the autocomplete list of all cars starting with the letter combinations entered, alphabetically, should be proffered. 

...Over the years this failure to is aggravated by new features that never optimize extant ones, and five years in you have an expert system no one can understand, totally unintuitive, hated by all users, but tolerated because "fucking computers." Ahem. 

### Regional Vendor Hegemony

The part about non-integration dramatically slows progress, because new vendors with great ideas have the worst time starting out because everyone views innovation and usability as a threat (and it IS). And police chiefs and administrators are by nature conservative. So they don't want to rock the boat. Instead, they go 'Nobody got fired for buying [X]' approach, buying what the agency near them bought. THIS is why there is regional hegemony in LE tech, also why innovative companies like must fight so hard for market share. 

Another reason for regional hegemony: certain agencies: NYPD, LAPD, Fort Worth among them, serve as Beta customers for new things. When NYPD or Ft Worth buy a tool, Every agency within 500 miles gets a sales appointment. That's Keeping Up With The Joneses, and it works well. 

### CJIS Stands For: The Elephant In The Room
  
Then we have the issue of Criminal Justice Information Services or CJIS, which is nominally overseen by [FBI](https://www.fbi.gov/services/cjis). All evidence and generally all case information must be stored in CJIS compliant systems, but getting approval for that is literally a 50-state problem. Vendors must demonstrate compliance with one main ruleset and 50 state interpretations... 

Not only does CJIS approval in Texas not help you in, say, Indiana or NY, but the path forward is different in each state, too. And you'll get absolutely nowhere until the state CJIS folks are cool with your whatsit. And there is no CJIS checklist. BASICALLY, CJIS is a modestly stronger standard than PCI, but it's not a prescriptive tickbox like PCI. 

CJIS rulesets on a state by state basis are better compared to regional CULTURAL differences than to state technical standards. AWS learned this the hard, long, expensive way... 

Once you've got all that, now you only have to convince someone that it is better to spend the money that would buy a new Tahoe, or inherent bias training for 50, that the money is best spent with you solving a problem they have handled for decades by telling cops to do it. 

That last part is tough. Anyone selling tech into LE knows that no matter what the chief wants, the angriest sergeant can destroy you simply by not pushing it, or saying it creates an officer safety issue to use - that slowed automated citation writing tools for years. 

### Innovating In Law Enorcement Technology

Truly innovative LE companies must compete with terrible extant technologies and all those cultural and systemic issues. The problem is 10% technology, and the rest is cultural, political, and financial. This means starting up is very hard... 

To start successfully, I think[[2](#footnote_2)], one needs laser focus, great sales and marketing, clear differentiation, a great USP, police expertise in whatever you're selling, a YEAR of real user acceptance testing In Situ (the car or the station), and oh yes, $100 million. 

Consider that there are four and only four ubiquitous police technologies dominated by one vendor: Motorola radios, TASER from Axon, body cameras from Axon, and semi-automatic handguns from Glock. There are great competitors to three of those four, yet they dominate. Why? They had all those elements I mentioned. Consider Glock handguns, which engaged in a diabolical and brilliant campaign to BUY all your old guns to sell you their (arguably - and I mean arguably - superior) new guns. They broke S&W and Colt's 100-year duopoly. How? $100m and a good product. 

Of course, [Shotspotter](https://shotspotter.com) is a contender for the fifth, but I omit them because while a national brand, and largely uncontested, it's a high-ticket item which self-limits the marketplace. 

Shotspotter CEO Ralph Clark's genius was democratization of the product by converting it from perpetual license model to SAAS, lowering the cost by an order of magnitude and making operation easier and more efficient. If not for that Shotspotter would have died fast and quiet around 2012. But look where ShotSpotter got lots of its money? Motorola. That's a hugely important lesson: the tech can be GREAT and EFFICACIOUS and PROVED, but you still need the $100 million. 

There are other examples. It could be argued that [Cellebrite](https://cellebrite.com) is the big brand in digital device forensics, with a more innovative company, [Magnet Forensics](https://magnetforensics.com), nipping at their heels. It could be argued that [Vigilant](https://www.motorolasolutions.com/en_us/video-security-access-control/license-plate-recognition-camera-systems/vigilant-platesearch-lpr-analytics-software.html) (now Motorola) dominates the LPR location and analysis space, etc. But none to the deep and wide extent that those four products dominate nationally. 

### The Market Is Just Fine...

That doesn't mean people can't make lots of money in LE tech. Just that it is a regional slog. It's also a market that is both highly fragmented into about 18,000 pieces, with confusing lines of demarcation of regional hegemony. 

And remember, your competition is usually a manual process and a spreadsheet. There is a book called Better Policing With Microsoft Office. To a chief, this is a FREE solution to the problem you seek them to pay you to solve - cops are a sunk cost, and to add to that: 

Cops is the only place economics generally don't matter. A cop spending 600 hours doing something is fine - there's no profit motive. it doesn't matter if it takes two years to investigate a murder because the result desired is closing the case - money is literally NOT an issue. 

Ask cops how much it costs to investigate a murder, or roll SWAT, or send more cops somewhere and they CANNOT ANSWER - it's like asking the cost of moving an aircraft carrier to the Gulf of Sidra. They're out there anyway. Yes there are incremental blah blah blah not the point. 

If the USP you have is saving the agency TIME? Forget it. You're done. You need to make police work BETTER. SAFER. More EFFECTIVE. If you can't, your fancy UX is WORTHLESS. If you can, and can make it efficient and easier and nicer to use?

That and $100M gives you a shot. /fin 

<a name="footnote_1"></a>[1] by "great reports" I mean reports that contain the right number of facts and statements and names and ID #s. I do not, hahahahaHA, mean well-written or compelling report-writing. That would be silly. 

<a name="footnote_2"></a>[2] I *think* because having only raised $3.5mm, and having to learn the rest by doing, I personally crashed the airplane that was my LE tech company into the side of a mountain, in conditions that were clear and visibility unlimited. 
