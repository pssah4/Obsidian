---
Summary: OpenAI-Produktstrategie, Entwicklung und Rolle von KI-Agenten
Content Type: Podcast
Content Creator: Azeem Azhar, Kevin Weil (OpenAI CPO)
Source: https://www.exponentialview.co/p/openais-cpo-on-building-at-the-cutting
Date: 2025-06-04
tags:
  - AI
  - Produktentwicklung
  - Agenten
  - Innovationsmanagement
  - Technologieintegration
  - Softwareentwicklung
  - Digitalisierung
  - OpenAI
  - Codex
  - ChatGPT
  - Automatisierung
  - Content
---
---
## Wichtigste Aspekte

- OpenAI hat **sechs neue Produkte** auf den Markt gebracht, darunter **Daten-Connectors** zu Google Docs, Gmail, SharePoint, OneDrive und weiteren Plattformen.
- Die neuen Connectors ermöglichen **Read-only-Zugriff** auf persönliche und Unternehmensdaten, um den **Kontext für ChatGPT** zu erweitern.
- Ziel ist die Entwicklung von **KI-Agenten**, die nicht nur Fragen beantworten, sondern eigenständig Aufgaben erledigen und wie ein digitaler Mitarbeiter agieren.
- OpenAI verfolgt eine **iterative Entwicklungsstrategie**, bei der verschiedene Modelle (z. B. O3, 4.0, Codex) parallel weiterentwickelt und getestet werden.
- **Evals** (Bewertungsverfahren) werden genutzt, um Modellfähigkeiten entlang verschiedener Dimensionen und Anwendungsfälle zu messen und kontinuierlich zu verbessern.
- Die Nachfrage nach **Coding-Anwendungen** mit KI wächst überdurchschnittlich (**75 % Quartalswachstum** laut SimilarWeb); OpenAI setzt daher einen Schwerpunkt auf Softwareentwicklung und Automatisierung.
- **Demokratisierung von Coding**: Ziel ist, dass künftig eine viel größere Nutzergruppe selbstständig programmieren kann.
- Kooperationen wie mit **Johnny Ive** zeigen OpenAIs Ambitionen für Design- und Hardware-Innovationen.
- OpenAI sieht die Plattform als **Enabler** für Drittanbieter: Je mehr Grundfunktionen die Plattform übernimmt, desto mehr Raum entsteht für Innovationen von Entwicklern und Startups.

## Thesen, Argumente, Erkenntnisse

### Strategische Ausrichtung & Vision
- **KI-Agenten werden als digitale Mitarbeiter positioniert**, die eigenständig Aufgaben erledigen und nicht nur auf Befehle reagieren.
- **Iteratives Deployment** neuer Modelle ermöglicht schnelle Entwicklung, Test und Markteinführung von KI-Funktionen.
- **Fokus auf User-Kontrolle**: Nutzer sollen jederzeit Einfluss auf KI-Aktionen behalten, insbesondere bei autonomen Agenten.
- **Plattform-Ausbau als Ökosystem**: OpenAI sieht sich als Basis für externe Innovationen und Produktentwicklungen.

### Technologischer Wandel & Marktdynamik
- **Technologische Entwicklung bei KI verläuft exponentiell schneller** als bei bisherigen Technologiesprüngen.
- **Jüngere Nutzergruppen** bauen Prozesse von Grund auf mit KI, während ältere Nutzer bestehende Prozesse mit KI anreichern.
- **Coding als Schlüsseldisziplin**: Leicht prüfbare Ergebnisse, hohe Marktakzeptanz, große Innovationswirkung.
- **Demokratisierung von Softwareentwicklung** wird als zentraler gesellschaftlicher Hebel betrachtet.
- **Schnelle Lernzyklen** und datengestützte Evaluierung (Evals) werden als Innovationsmotor verstanden.

### Produktentwicklung & Forschungsansatz
- **Zusammenarbeit von Forschung, Produkt- und Engineering-Teams** führt zu schnellen Produktinnovationen (z. B. Deep Research).
- **Evals** dienen als neues Messinstrument für Fähigkeiten und Produktqualität, ersetzen klassische Produktanforderungsdokumente.
- **System-Prompts** und deren Gestaltung bleiben für das Verhalten von Modellen zentral, sollen aber langfristig an Bedeutung verlieren.
- **Hardware-Innovationen** (z. B. in Kooperation mit Johnny Ive) ergänzen die Softwareausrichtung und adressieren Limitierungen aktueller Geräte.

### Marktchancen & Wettbewerb
- **Plattformstrategie**: Je mehr Basisfunktionen OpenAI als Plattform bereitstellt, desto mehr Freiraum entsteht für Startups und Entwickler, innovative Lösungen zu bauen.
- **Kritischer Erfolgsfaktor für Gründer:** Produkte sollten an der Grenze der aktuell möglichen KI-Fähigkeiten gebaut werden, sodass sie mit den nächsten Modell-Generationen weiter aufwertbar sind.
- **Wachstumstreiber**: Chatbots und Coding sind die am schnellsten wachsenden KI-Anwendungsbereiche.
- **Wettbewerbsfähigkeit** chinesischer KI-Anbieter steigt, westliche KI-Labs sollen demokratische Werte als Differenzierungsmerkmal sichern.

### Ausblick & gesellschaftliche Wirkung
- **Künftige Hardware- und Softwareintegration** wird neue Interaktionsmodelle ermöglichen (z. B. ambient intelligence).
- **AGI** (Artificial General Intelligence) wird als kontinuierlicher Prozess mit schrittweisen Fortschritten verstanden.
- **Breiter Zugang zu KI** gilt als gesellschaftlicher Mehrwert, z. B. durch Unterstützung bei Alltagsproblemen (Gesundheit, Coaching).


---

### Transkript

```
I think we can formally get started, Kevin, so I will do a little bit of a top of all of this. Well, hello, everyone. I'm Azir Mazar, the founder of Exponential View, and every week we host a live conversation with what is happening in AI and what it means for you.

0:17

Now, today I'm so excited to welcome Kevin Weil. He is the Chief Product Officer of OpenAI, coming off the back of a storied career in companies like Twitter and Facebook. Facebook. So much to talk about. So first of all, Kevin, thank you for making the time. You've been busy today already.

0:36

It's morning in San Francisco and you've already launched some things.

0:40

Yes, we have. And thank you so much for having me. It's my first live Substack, so I'm excited.

0:45

Well, hopefully many more to come. You are really keeping us on your toes. And so just an hour before we went live, there was another spate of product launches from OpenAI. What do they tell us about your vision for ChatGPT and where the product is going?

1:00

Yeah, well, the biggest thing that we launched this morning, we launched like six different things this morning, but I think the most important one kind of for the long-term future of AI is we launched a series of connectors that can connect to your either personal data or if you're an enterprise, your enterprise data.

1:19

So this is connectors into Google Docs, to Gmail and Calendar, to SharePoint, to OneDrive, uh dropbox box linear all of these different tools that you use every day to get things done with the rise of our reasoning models connecting them into the the

1:38

services and the data that you that you use helps the models be way more useful so it's not just that you know you can now ask if you if you you know at work for example if you connected in if you're google docs or sharepoint You connect it into the docs that you use every day. Suddenly,

1:54

ChatGPT can get all of this context on the enterprise and on the state of projects and on the latest about any particular thing that's going on. You wouldn't ever have an employee at your company that you didn't give access to docs. It's like where the conversation and the strategy and other things are happening is

2:13

So now you have ChatGPT that has the ability to do it. And today these are read-only. They're read-only, so they're able to access the information but not create on the other end. But you can imagine going forward, another big part of this is that

2:30

these should these that chat gpt should be able to take actions should be able to help you write a document or create a presentation or you know write tasks to your tax management system and ultimately combine all of these together to begin really working like an employee

2:46

Right. So that's the hint, right? That direction of moving ChatGPT from something we interact with, with a challenge and response, into something that is more evolved and feels like it's really doing work for us as an employee. We're going to spend some time digging into that. It's such a big vision. Let me ask about you.

3:07

You're the chief product officer of what I think is the most important company in the world today. So how does that feel like to you, day to day and week to week?

3:18

I mean, it's a privilege. It's the most exciting place I've ever worked. And I've been very fortunate in my career to work at a bunch of awesome places with really great co-workers. But I think... You know, the opportunity in front of us,

3:31

the rate at which AI is changing all of our lives means we have we have an ability to make a really big impact and we take that super seriously. So I get to work with amazing colleagues. I get to kind of, you know,

3:45

have a front row seat to the way that our models are evolving and that the way this is all impacting our lives. And hopefully we get to build some products that that make a difference in your life and in the lives of everybody listening here.

3:58

Well, nearly a billion people have made, at least voted with their mouse finger to use ChatGPT just since November 2022. Technology always changes us. The television did. We got TV dinners and we got water cooler discussions. The internet obviously changed us in different ways. Cars as well. We got big box retail. We got the suburbs.

4:25

We got the picket fences. Desperate housewives. How might AI products reshape our everyday life?

4:34

Well, I think one of the other interesting things you get when you have these waves of technology is you start by doing the thing that you were doing with the previous wave, but sort of with the new medium. The first TV advertisements were people standing on a stage reading their radio advertisements.

4:51

And then people slowly figure out that you can actually do what we have as commercials today, which are much more interactive and sort of dynamic. And so we're still probably in that mode of people... when they look at the impact that AI can have in their lives or in their work, they're kind of like, okay,

5:09

I have these processes. How do I, you know, sprinkle AI on top of this to make it better, faster, etc. And like, that's fine. That's all good. But I think the power will come from, as in previous technology transitions, the power comes from completely reimagining

5:28

work that you're doing from first principles using the new technology um you know so mobile wasn't just about uh you know a computer in your pocket it was you know you have access to gps and you have these totally you have notifications and

5:43

totally new ways to interact with uh with technology i i think over the next you know year we're all going to be in the process of reinventing the way that we do things with AI. And the fun part is the technology is moving so fast. It's not, I mean,

6:01

faster than any technology I've ever worked with before I've ever seen in my career. So even as we're reinventing, the technology is gaining new capabilities and it's just, it's an exciting time to be alive.

6:12

I mean, that rate of change is quite something. I was looking for something today which I know would not have been possible four months ago. So I was using O3 to help me find a little portable mobile 5G router for when I travel and I just need to get a good quality signal. And of course,

6:32

O3 went into all the technical specifications of the radio frequency chipset and said, well, you know, this earlier... Ruta has got a slightly better Qualcomm chipset they no longer use, and you'll get one extra signal bar in rural environments in the US, but not in Europe. And I'm thinking that sitting there going, this is kind of insane.

6:53

But I'm really curious about those types of behaviors. What are the surprising behaviors that you've seen emerge around ChatGPT from your users? Sam has sort of talked a little bit about generational differences, but give us a flavor of things that you've learned about behavior that are just

7:10

really hard for product teams to research or figure out a priori.

7:15

Well, I do think, I mean, Sam has talked about the way that, like I said, the people today, I think a lot of people are sort of sprinkling AI onto their existing workflows. And it's young people that are you know, there's sort of this is native to them in a way that it's not native to, you know,

7:33

those of us who grew up without AI. And it's, I mean, my kids just, they're like, of course, you can talk to a super powerful AI that like, you know, can customize itself and answer any question you have. And kids that are graduating college these days, as like engineers, are like,

7:54

they don't know any other way to write code than using you know, AI editors like Cursor and Windsurf. And it's just completely natural to them. And so it gives them superpowers in a way. And it's one of the reasons that we look a lot at how our youngest users and our young users, you know, late teens,

8:12

college users, things like that, are using the product because it teaches us a bunch.

8:17

Can you characterize those differences, though? So what is it like if you're in your early 20s, you're using ChatGPT, how does it feel different to somebody who might be in their mid-30s or early 40s?

8:31

There's sort of an always-on nature. You just... you realize that you have this super assistant in your pocket that can not just answer any question, but it can teach you anything that you want to learn. And so when you go about life that way, the rest of us are like trying to remember, you know,

8:51

trying to think about the processes that we go through and how we can reimagine them. If you're younger, you might not have had those processes. And so you built them from the ground up with AI. And so it's just a core part of the way you operate your life.

9:07

And in some ways, they're ahead and the rest of us are catching up.

9:12

A lot of people are scared of this technology. A lot of people are nervous. I've just come back from Brussels and spoken to people in a different sector, and you do get that sense of fear. What could change in the product to address that?

9:33

I think one thing that I think is really important is people ask, you know, what, what, what should I do about AI? How should I think about it? And my answer is always just use it. And, you know, of course I think everybody should try chat GPT, but whether it's us or any of the others,

9:50

just start using it because you, it's the number one way to realize that this is, it's not this like super scary thing that you read about. It's, it just helps you get more done and you're like, oh, this is great. I,

10:06

I now have this like incredible new like thing that can be part of my life and help me get things done and help me like automate a bunch of the like boring work that I have. Right. So, the number one thing is just start using it. Also, given the rate that the technology is improving,

10:22

if you don't start using it now, it's going to be even harder to sort of catch on to it. And if you believe that AI is going to be a big part of our lives, that's not a train you want to miss. So that's the number one thing. Just start using it. But then we think a lot,

10:36

especially as you get towards agents and other things, we think a lot about making sure that the user is in control. So you don't want the you know as you're getting to to use chat gpt or any other ai you don't want it

10:51

to go off and do a bunch of things for you without you you know feeling in control and so it as you know it's one thing if it's like answering a question for you reading some docs and summarizing them things like that but as we're in this this transition from chat gpt being a thing that

11:09

answers questions to a to a product that actually goes and does tasks for you in the real world and you should be in control of any actions that it takes and over time as the models get better and you begin to trust them more than sure you can

11:22

give it you know sort of more leash and trust it to take more actions autonomously but you should control that every step of the way and i think that's one of the most important ways that we're looking to build trust

11:32

I mean, there's a lot that will change as you move to more and more of these agent-based workflows and the models be able to use tools. And I guess we have to co-evolve. Definitely, we should look into those questions. I'm just curious about your own experience. A lot of us have these oh, shit moments when we use

11:52

right there's there's something sublime that happens or there's two years of your work that gets returned in in five seconds um what was your most recent oh shit moment using using your own products

12:05

Well, so I'll give you, this one's a little bit more, I don't know, pragmatic, but it was a really meaningful thing for me. We have, we were talking about kids as people were sort of coming on. And our, our, one of our sons had a minor surgery. And

12:26

It was it was one of those things where all odds were that it wasn't going to be a big deal. But there's a small chance that it was a really bad thing, you know. And so they they do the surgery and like they take the thing and they go to biopsy it.

12:42

And you're waiting for you're waiting to hear back. And as a parent, you're nervous, even though, you know, logically that the odds that it's anything bad are really small. And at some point we got a letter in the mail. with a bunch of you know doctores on it that looked pretty intimidating frankly you

13:03

know there were a bunch of words i didn't understand and and the characterizing what this thing was and it wasn't it didn't say like you should worry about this or you should not worry about this it just like characterized it and then you know

13:15

finished and i couldn't get a hold of the doctor she was in surgery or something you know and so there i was like oh my god what does this mean and so i took a picture of it i put it in chat gpt and i said like should i be

13:28

worried and and and i said like can you explain this to me like i'm five right and and chat did it and was like no this is totally fine everything like nothing to worry about and i actually ended up not being able to get a hold of the doctor for

13:43

72 hours because she was just super busy and that 72 hours would have been a terrible 72 hours for me as a parent if I was just sitting there brooding. And ChatGPT was able to answer. And that's like, that's, you know, us with like access to great healthcare.

13:59

You think about the impact of this all over the world where people don't have the same access. It's really powerful. And I think that's sort of an underappreciated part of ChatGPT.

14:10

I mean, that is a wonderful story, and I'm glad that your son is healthy and comes out of that well. But it also speaks to the power of this particular product, right? It's a really complex, complex product. And there's no way I can talk to you without asking you about how that complex

14:30

product finds its way in that funny dropdown in the top left of GPT. There must be something. You guys are all so brilliant. There must be some internal joke about, Well, how should we order it? What should we call the next one? You know, what's really going on there? What's really going on there?

14:48

And, you know, shouldn't we all just be using 03 and 40 if we're in a hurry?

14:55

Yeah, it's a totally fair question. And you can also, you can and you should make fun of us for our naming as well, which is, you know... But it kind of comes back. So we have this philosophy of iterative deployment, which is these models are, I think AI is going to change all of us.

15:18

It's going to change the world. It's going to change society. And we believe that the best way to do that is to kind of co-evolve together. is to get these models out there and put them in people's hands help them understand and also you know they help us discover the capabilities of the models

15:35

and the weaknesses and other things and so we we sort of learn together and can iterate really quickly and improve um so that's that's part of it the other part of it is we're we're building a lot of new capabilities as we go and if you if we took the time

15:52

to only you know we just had like one model and we just had to build everything into one model we'd end up moving a lot more slowly and you know things would be simpler for sure but we'd end up moving a lot more slowly because sometimes it's

16:05

easier to build a new model with a certain set of capabilities that's great at certain things not as good at other things and so together you have sort of a a collection of models that that can do lots of things each individual model has its strengths and weaknesses. And so basically,

16:21

we've optimized for going faster and getting more capabilities in people's hands at the expense of a bit of confusion. And then over time, as we sort of gain more control over some of the new functionality, we understand it better, we build it back into the core model.

16:40

So you have models like GPT-4 that can do a lot of things well. And this is what we're trying to do with our forthcoming gpt-5 is take a lot of the things that we've learned and build more of the capabilities into a single model so that it's easier for people to reason

16:58

about it's like what model do i use just use gpt-5 right and you know in a perfect world it knows how hard the question you ask it is and so it knows whether it should give you an answer like this or whether it should think for a while And, you know, that's what we're shooting for. And,

17:15

you know,

17:16

in a way, that's lifting the cognitive load that is currently on the user because I will sit there and I'll think, do I have time? Is that a complicated question? Does it need to go to the reasoning model 03? Does it need a longish prompt for 03?

17:29

Because it might get the wrong end of the stick if I give it a shortish prompt. And in a way, what you're talking about is crunching that all and building it into the model itself.

17:41

Yeah. And and look, what I don't want to do is over promise and say, oh, in the future, like we'll only ever have one model and it's going to all be simple because we we're also, you know, say we launched GPT five. We're then going to have a bunch of new capabilities beyond that that we're trying

17:57

to build an experiment with. And we're going to want to get those out to people and deploy iteratively and so on. So I expect you always have this sort of phenomenon of there are new models, and you've got sort of your workhorse models, and then you've got some of the new ones that have certain frontier capabilities

18:14

that we're experimenting with and learning with together. And then over time, as those mature, they all kind of get merged back into single models.

18:22

So it seems that a lot of the velocity is actually about getting through the loop, right? The learning loop. And you just run all these horses at the same time so you can gather enough data about what models work against, what capabilities. So you've In a way, that helps you develop and deliver on GPT-5,

18:41

and I hope you'll share the date with us. Down to the minute. Down to the minute, yes, so we can time ourselves. But does that also mean that, you know, how far out are model capabilities being delivered? Are there things that are being worked on today that might not make their way into models until mid-2026? Yeah.

19:04

Yeah, it's a good question. It's one of the most interesting things about working here is you kind of have a sense of what's coming. And, you know, I'm not in the research team, so I'm getting this, you know, as I collaborate and work with the researchers. I would say, like, you know, on the product side,

19:23

we have a decent sense of what's coming in the next, say, three months. maybe a hazy sense over the next six months. And beyond that, it's harder to say. You know, you have a certain set of capabilities, you know, where like, you know a bit, but you see things coming through the haze a little bit.

19:42

And sometimes, sometimes capabilities are, you know, it's research, right? So it's not like you just, you have the formula and you just turn the crank. It's, we're uncovering new things and it's unpredictable. So sometimes things take longer than expected. Other times you see these capabilities that you didn't expect at all that are kind of emergent.

20:01

And all of a sudden something just works.

20:04

Can you give an example of one that just worked that you weren't expecting?

20:08

Well, I mean, deep research is an interesting example where, for a while, there were a handful of researchers thinking about the... It was like, okay, we could probably make the model able to do this iterative... kind of research where you know with deep research you give the model a arbitrarily

20:29

complex query to go research something that would probably take you a week and it will go off and it'll go off and do like a hundred searches but not all at once it'll do it'll do three or four or five and then it'll reason about the results

20:43

that it gets back try and understand how they pertain to what you asked and what gaps are still there and then we'll go off and do some more searches and maybe think again Maybe it'll write some code for a little while, as it thinks, and then go do some more, you know.

20:56

And so it's this sort of iterative, I mean, it's what you would do if you were, if someone made you write a very complex research report. You wouldn't, you go do some research.

21:04

Sorry, Kevin, I don't do that anymore. I just go to deep research. I actually can't remember how to do it on my own. But yes, I understand, right? You have to, you sort of inch your way across and you figure out exploration strategies and go down to dead ends and come back.

21:18

Yeah, and so to your question, that was something that some folks were like, okay, this is coming together. But it's not clear exactly when it will come together. And so there was a small team of researchers that just believed in this and were working to make this real. And for a while, it wasn't good enough.

21:38

It wasn't good enough. And then there was some advances. And all of a sudden, you're like, OK, this is getting good enough. And somewhere in that time frame, we put also a product and engineering team working on it with them And then you have the thing that I think really is the magical part of open AI.

21:58

When you get a research team and a product and engineering team just in the same room, all bringing their unique skills to bear and you understand the problem you're trying to solve. And so you're bringing back use cases, creating evals and benchmarks for how you measure whether you're successful against those use cases.

22:16

The research teams are taking that and using that to improve the model itself. And you get this tight loop of the model improving towards a particular product. And it's, you know, I think our best products are the ones that we build that way. And deep research is a good example.

22:32

That's a novel way of thinking about product development. I mean, if I think about the history of product development, quite often it was before the 90s, before the consumer internet was run by engineers and they'd say, we've got a new chip that can do this.

22:47

And you then try to figure out some software that can do useful things on that chip. I think the big breakthrough of the consumer internet was to put product managers at the heart of of product development. And we talked about lean and iteration and being very data-driven and user-centric. And now you're getting to this new model,

23:07

which I would characterize as not at all a return to the pre-internet product engineering-led, but something that is quite novel because the researchers discover something that's a little bit a new capability. And then you have to have a very rapid discussion about how can that capability be productized. And then this word you used, eval,

23:28

which I guess it means how can it be measured to see whether it's actually doing its tricks. So is it really a new discipline that is evolving at this point?

23:38

I think it's a completely different way of building products. It's certainly different than anything I've ever done in my career. And, you know, within research, there's kind of a spectrum, right? There are parts of our research team that are just like deep research. It's almost academic in nature because they're trying to just like,

24:00

they're looking for new breakthroughs. They're trying to find things that nobody has ever, you know, figure out things that nobody's ever figured out before. And those kinds of things, you don't want to be product-driven at all. Because you want to give a lot of room for exploration and fundamental breakthroughs.

24:18

And then there's kind of the other end of research. It's more on the post-training side where you really are trying to teach the models to do specific things very well. And those teams tend to be much more like you know, partnered with product and engineering teams with a common goal.

24:37

And then it's kind of a spectrum in between. And, and so I, I think the right way for us to be is not, we certainly don't want to be entirely product led. That's not that's not the magic of this place um it's not maybe entirely research-led either

24:55

because it's good to know you know feedback about what problems you can solve for people and how we can make the biggest impact in the world it's really sort of a combination of both with research really at the core though um and i like i've

25:08

loved it it's it's the most fun in the world um yeah and you know moves super fast. Computers can do things that they couldn't do two months ago and we're constantly in that state.

25:21

But when you're working with research, then it's more than just looking at a scaling law and saying, oh, we've just, Sarah Fry has just signed off another 100,000 GPUs. Therefore, it will be able to do this in six months when the trading run is done. There's more to it than that.

25:37

But one of the things I find fascinating is how do you map those capabilities against products. And you talked about evals, which I guess are evaluations. What is the structure of an eval? And is it what replaces what was in an old product requirements document that we might have had 15 years ago?

25:57

Yeah, sort of. I think in some ways for understanding where the model is good and where it's not. If you think of the model as sort of an intelligence of some sort, Intelligence is so multifaceted. people are smart in a million different ways, and one smart person is better than another in certain areas and worse than another.

26:22

So one way to think of evals is a way to measure capabilities and intelligence of models on different dimensions. So you can have evals around how good it is at solving USAMO Math Olympiad-style problems, and another around how good it is at chemistry, and another one about how good it is at creative writing.

26:45

But are you using the public benchmarks for that? The sort of RKGI and Amy and GPQA as your way of measuring?

26:55

Some, and then also when we're building specific products, I think one of the most effective ways to build products is to take the skill that you want the model to have in order to meet the product need and turn that into an eval so you can actually understand how good you are at it and also how you're

27:13

getting better over time. But one of the fascinating things is the evals that we all used a year ago to measure models, they're all very kind of cut and dried. Like you're testing against math. And with math, there's a right answer. You can talk about creative writing evals, though. And with creative writing, there's no answer.

27:39

So how do you grade that, right? That's one problem. The other is like, as you start to take on more complex tasks, you're not just answering questions. you're actually trying to automate some multi-step workflow, there may be ambiguity in the right way to do that.

27:58

If I'm an AI booking a flight for you, there's not a single way to grade which correct flight. And so... So you also get into these really interesting, challenging, subjective ways of how do we actually grade this particular task? And part of having an eval, if you want to at least automate it,

28:17

is you need to also have a grader for it so that you can very quickly understand how you're doing on that eval. So it is interesting. It's one of the skills that I think is going to be more and more important for PMs over time is the ability to actually create evals for the products that you're building.

28:33

Yes, I mean, that's one. And the other one is the prompt at the front end. Because what we are starting to see with these leaks, and I don't know how real they are or not, but there are a number of X accounts that say, I've just had the leaked system prompt over then insert your favorite foundation

28:51

model or coding tool. And the system prompts, which are the sort of structured instructions that go out with every query, are really, really quite complex. I mean, they're product in of themselves now, right? They run to thousands of words. They're highly structured. There's clearly strategies being applied as they get put together.

29:12

So how important is that skill and capability when you're shipping products to people like me? Can you say it one more time? I just, I broke up just a sec. It was, yeah, yeah. It was just, it was this, how important is that capability of the system prompt design in designing effective

29:29

products for people like me to use?

29:33

Yeah, it's, I mean, actually more than, more than people realize, I think. I would love to make it over time less of a thing. And I think over time it is like, If you go back a year or two, everybody was talking about prompt engineering and it was going to be the skill

29:51

that everybody had to master in order to do anything with AI. You don't hear about it. You don't hear it talked about quite as much like that. And I think that's a good thing. Ideally, it matters less and less that for any particular user, if they have a question, they want an AI to do something for them.

30:09

You shouldn't need to get into like arcana around, did I use the exact right word? And did I give my exam? You know, it should just work. I think that's part of increasing intelligence is the model can understand what you're looking to do and do a good job of it without you having to work super hard

30:25

at it. That said, prompts still do matter and the models are very controllable with prompts. And so, you know, we still find we'll launch something and we'll find that it's not behaving in certain ways the way we want it to. And we can adjust it with a prompt a lot of times.

30:41

You don't need to go back and like retrain the model. So it's both that I want to make it less necessary over time and that it is still a powerful vector.

30:50

Well, these are two of the vectors of the direction of the product, but the third one is the idea of agents and what agents will bring to us. I think probably the first agent product that OpenAI launched that I used was deep research. And the word agent is being thrown about quite a lot. I mean,

31:12

I'll use the word agent, and what I mean is I've strung a bunch of prompts together through your API, and there's a bit of logic to move... you know, a document through a series of steps to the other end. What does an agent mean to you?

31:26

We think of an agent as something that can do independent work. So it's not just a quick, you know, you ask a question, you get an answer, but it's actually off doing tasks for you in the real world. So another, I think deep research is a great one where it's off doing, you know,

31:40

hundreds of searches and putting together a complex report for you that might have taken you a week. I think another is Codex, which is our software engineering agent that we just launched. And the for that product the you know what you can do is just if you have a code base

32:01

that you're um that you're operating against you're building a new feature in a code base or debugging something you can just give this agent the prompt like hey i need you to fix this thing i want you to do this to the background of my web page i want you to you know build this new feature and

32:17

It will go and look through your entire code base, understand all of the context. If you're, you know, fixing a bug, it'll go try and figure out where that bug exists. And then it will write new code for you and create a pull request, like a diff, you know,

32:32

here's a set of changes we need to make to the code. And then you can go review the code. And the agent did the whole thing. And so, you know, I used to be an engineer. I still write code a little bit in my spare time, but I haven't written a single

32:47

you know, line of code for open AI. But with Codex, I was this was like, you know, a few days before it launched. I was, you know, it was like 11 at night or something. I was doing a bunch of work that I had to do before I could go to bed.

33:00

And I was like, you know what, I bet I could fix a bug right now. and uh and so went and found uh a bug that looked relatively simple um and just you know pasted the context into codex said can you go off and fix this bug by the way

33:17

it was in a language that i had actually never worked with in my life so it would have taken me even more time if i had to do it myself and 10 minutes later i had a pull request it looked reasonable I submitted it. An actual legitimate engineer looked at it and said, yeah, this looks right. And,

33:36

you know, now there's a few lines of code shipping today that, you know, came from me using Codex. And it's like, It speaks to the power of this thing when you can just have this software agent off like actually solving real world tasks for you. And in the meantime,

33:53

I was like writing email and following up on Slack and, you know, doing all the things that I do in my day job. So it was just purely additive, which I think is really cool.

34:01

Yes, because the codex process takes a little bit of time. It has a lot of material it has to read and understand and then make the changes. And I'm curious about, this is a question that everyone who's built a product that does code automation or developer augmentation is asked is,

34:19

so today what portion of the OpenAI code base is in the first instance produced by codex rather than by a human engineer?

34:31

Yeah, it's pretty meaningful, and it's increasing quickly.

34:33

Right, okay. Somewhere in the meaningful. I'll go up and ask 03 what meaningful means in percentage terms, and I'll get a good distribution there.

34:45

The cool thing is you can fire off 10 of these tasks at once, right? So we try and actually give you the value of all this parallelism. Um, where, you know, it's not just, you can do one thing, but if you have a codex agent working for you,

34:56

why not have 10 codex agents working for you on 10 different tasks?

35:00

Right.

35:00

Um, and by the way, just to connect it to the previous topic on evals, um, this, this is also evals are, are, there's a, there's a really important kind of subtlety to them too, where they have to be tailored to the product that you're trying to build and the problem that you're trying to solve. Um,

35:20

where you know coding isn't one thing just coding is a small vertical of the entire world but even within coding you can be good at lots of different kinds of coding and um with codex that that was a great example of of going and saying okay what

35:37

what kinds of coding really matter to us what kinds of tasks and all the tasks that a developer does what kinds of tasks do we really want to be good at and we created evals for those and then we We made sure to monitor as we trained the model,

35:50

is it getting better and better and better at these? And, you know, you go and accumulate tasks and examples for the model to learn from. But you do it against a specific set of evals that correspond to a specific set of problems you want to solve. So I just thought it might be a good example of...

36:06

It's very capability-driven in that respect, right? And then it speaks to, you know, how do you actually... do enough testing, both to make sure that you are, you know, getting to the level, the right level of score that you want, but also making sure that it doesn't go off the rails, right? And, you know,

36:22

I think that as these agents get more and more complex, given more complex tasks, that's something to bear in mind. I mean, in one of my workflows, which was a very, very simple one where I wanted an agent to go through and grab some data from a series of web pages and populate an Excel spreadsheet.

36:45

And I was using some third party agent framework. And it was so diligent, Kevin, that it said, I must check my work. which it did about 400 times and left me with a $75 bill. And it had got it correct the first time, right? It got it right and stuck in this strange loop.

37:02

So that's one of the things I think that I hear when I go around people saying, well, how are we going to be able to control these things? Not from a, you know, a humanity out of control method, uh measure but from a enterprise reliability how can i make sure that this isn't

37:19

like the sorcerer's apprentice and the the thing runs runs out of control when i've simply asked it to book one flight to italy and it's booked me 200 and how do you

37:30

test for all of that yeah i think part of this is about making sure that like we talked about earlier that the user is in control here so You should be able to at some point be like, hey, you know what? You've checked enough. Like, you're good.

37:46

And the other interesting thing in all of this is the technology is evolving so quickly, much more quickly than I think we're used to with technology. We're used to things taking like decades to deploy and to really achieve scale. one of the, the, the phenomenons you see with AI technology is there'll be, there'll be some benchmark,

38:11

some eval that were, that AI just, you know, can't crack. And people are like, oh, AI just can't do that. And, And then one day, somebody ships a model that gets like 5% on that eval. Still mostly can't do the job, but just like begins to get it.

38:32

And then what you inevitably find is like two months later, there's a model that's at 30 on that eval. And then four months later, there's a model that's at 60. And then, you know, within six months, it's completely saturated. And like models are great at that new skill and will forever be.

38:49

And so you go very quickly from like proof of existence to like, oh yeah, of course AI models can do that. And that like rate of development is still... I think, something that we're not totally used to.

39:03

It's that first one or two percent, right, that becomes hard, proves it can be done. It's the Kitty Hawk flyer. And then within 30 years, we're moving large numbers of passengers across the Atlantic. But in this case, it's within 30 days. So I want to ask about coding and coding agents. So did you

39:20

If you look at the growth of Gen.ai applications, and SimilarWeb had some data come out a few weeks ago. The baseline was that the generalized chatbots are growing at 25% per quarter. That's the chat GPTs and so on. Virtually every other product category, image generation, video generation, sound generation... is growing slower than that or declining in size.

39:46

And I view that as the black hole that is the capability of your core models. The one category where growth was faster, 75% a quarter, according to SimilarWeb, was in coding. So I was curious, have you selected coding... from a kind of commercial perspective because you can really see the demand and

40:08

developers are always willing to experiment or do you select coding because being a a testable structured verifiable set of outputs it's a slightly easier challenge than a sort of fuzzy amorphous tasks that occupy the rest of the world

40:26

Yeah, it's a really good question. And actually, coding is this vertical that kind of hits all of these things. For one, it's really important to us because if we can speed up coding, if we can make every engineer more effective... We also make ourselves more effective.

40:44

And so we can build even faster and we can bring AGI to the world faster. So it's interesting to us from that perspective. It's a clear kind of milestone or step on the way to AGI itself because it's a very sort of general purpose reasoning. It's also a relatively gradable task.

41:05

Like you can tell like in math or other things if you get the answer right. It's also something that our engineers are familiar with. So it's a problem space that they understand and have good intuition for. It's also a huge market, as you were saying.

41:19

It's also a market full of early adopters, you know, technologists leaning into this. It's also relatively sort of open and unregulated. It's not like trying to go into health or something where there are all kinds of other things you have to do. And so it's this aggregation of all of these interesting things that make coding a

41:40

really interesting market. And I haven't seen that data, but I totally believe it.

41:44

and and would you say uh that within coding are you already seeing signs of serving people like you who are not technically engineers anymore in other words we're seeing that expansion of the market through through these tools oh yeah and i i

42:00

think there's going to be so much value in in democratizing coding out to the world there's like what 30 million uh developers or something worldwide depending on how you define it um Which is great. That's a lot of that's a lot of people. But imagine if you can imagine if a billion people can write code.

42:17

I was talking to somebody the other day who was just telling me they were during covid. They were they were working for their local county trying to get, you know, vaccinations and stuff out to people. And they were trying to put together a website to track so people could like sign up and just do basic stuff.

42:39

And the whole world was busy and they just, they couldn't do it. They couldn't create a website. They didn't have the skills to do it. And as a result, they were, you know, managing things less efficiently, doing a bunch of manual work at a time when everybody was slammed. And he was just saying like,

42:53

can you imagine if I had these tools, we would have been able to create a website overnight. It would have just worked. And, you know, they would have been able to do their work more effectively. And you have that times a million as you look around the world.

43:09

And so, I mean, that is actually the other thing about coding that I think is super interesting. That's maybe like the, you know, ninth reason why coding is a good... It's such a general purpose technology. If you can create code, then you can create all kinds of things.

43:24

And so there's something really powerful to the idea that a billion people might be able to write code.

43:31

But it also speaks, though, I think, to how this may fundamentally change the software industry in the way that the internet changed the software industry, not just because of packaging and distribution, but the way we interacted with social technologies, right? My Microsoft Word, when it was on floppy disk,

43:51

never allowed me to sort of exchange notes with somebody else on like Google Docs. And one of the big questions that's out there is, as a platform company that is building the most performant models out there, how much space do you leave for startups? You know,

44:11

I remember when Microsoft introduced disk compression in Windows 95 or 97 or something, and there were a whole load of third-party companies that offered disk compression that essentially went out of business there and then. And this is something that happens on X every time you release a new foundation model.

44:29

It's like every time Kevin tweets, another 50 startups died. Where is there space, right? Where is there space in the software world, in the AI software world, which is safe from the increasing capabilities of foundation models that you and other companies are building?

44:49

So, Steven Sanofsky told me an interesting story about this one time. Steven used to run Windows at Microsoft and Office and, you know, everything. And he was telling me this story about, like, the transition from Windows 93 to Windows, or whatever it was called back then, to Windows 95, Windows 3.1, maybe. Yeah.

45:07

Where it was just, like, the beginning of the internet. And so most people weren't using the internet. And if you were going to actually... get on the internet with Windows 3.1, you had to go to some University of Oregon professor's website and download a TCP IP stack, compile it yourself, and install some device drivers,

45:31

and then you could actually go on the internet. and then in windows 95 of course the internet was happening and they were like okay we need to ship this stuff with windows and so they did and it was like you were saying there was this you know there were a bunch of people who were like hey now

45:46

that you know you've just like put that university of whatever professor he did all this work and now you just shipped it come on and Stephen's point was that you would never want to live in a world where today you still had to go to like some professor's website and download a TCP IP stack and

46:05

compile it yourself to get it going. You just want to use the internet. And basically the expectations of a platform, the consumer expectations of a platform... Are an increasing function of time. You should probably just provide that. And then those 10 companies can go do more interesting stuff. And I've always remembered that story.

46:44

It's really stuck with me. Because I think the fact that people are just going to expect more and more out of these platforms is very real. But the upside is all for third parties in this, for developers in this world. Because... If the platform provides more of the building blocks,

47:01

then they can spend less time re-implementing the wheel on these building blocks and more time doing the thing that they actually, you know, uniquely add value in. And AI is going to change absolutely everything in our lives. Any... Any industry, any vertical, any geography that you can imagine, AI is going to touch.

47:22

And so there's so much opportunity for developers to reinvent and reimagine. I think anything that we can do on the platform side to help accelerate that by making more of the building blocks easy, we should be doing.

47:36

So let's imagine my son, 20 years old, and he wants to build a product on top of OpenAI. Where is a good place for him to go and build it?

47:49

I mean, almost everywhere. There's so much opportunity. One of the things, Sam said this one time, and it stuck with me. He said, if you're building a company and you're building... at the frontier of of you know the model capabilities if you're building something

48:12

that really just barely works and and you can't wait for our next model because you know it's going to make your product sing then you're probably building in the right place because you're you're you're introducing something new to the world you're like making something possible that wasn't possible before sure and that's

48:30

where you want to be if instead you're building like some sort of scaffolding around that covers up the weaknesses of a current model, and you're actually afraid of our next model because it might not have those same weaknesses, that's a bad place to be building. Because on average, models are going to improve really fast,

48:49

and what's a weakness from one model will not be a weakness of the next. So I think the thing to be building is like what we talked about at the beginning, reimagining use cases from first principles, building them from the ground up with AI.

49:03

And if you're in a place where you're excited about the next model that comes out because that's what's going to make your product sing, that's a great place to be.

49:10

That's a fantastic heuristic, which is actually, if you're a founder out there, think about something that you want to build, that the models are not yet capable of, but will be capable in a little bit of time. And you can build on top of that capability.

49:24

We can't talk about products without talking about your new product buddy, Johnny Ive. So how... Tell us a little bit about what the mood in the office was when that lovely black and white photo was released.

49:41

Oh, people are incredibly excited. I mean, how could you not be? I use products that Johnny designed my entire day. And... He's been a part of building some of the most sort of cherished products and hardware that we use every day. How could you not want to work with him?

50:03

And getting to know him through the process and other things, he's also such a lovely human being. He is, for somebody who's accomplished so much, he is so humble, thoughtful, kind, soft-spoken. And then, you know, he'll say something sometime and you'll be like, oh my God, like that is a completely different way of looking at the world.

50:28

And that opens my eyes to something that I just had never thought about. And so is this combination of like genius and also wonderful human being How could you not be excited to work with him?

50:41

And of course, he's a Brit. How is his group and your group going to work? How are you guys going to interface?

50:50

Well, I mean, he's coming in focusing on these sort of consumer hardware products. And then also over time, I think will play a very significant role in design as a whole at OpenAI. And again, I'm very excited about that. How could you not be? Johnny Ive coming in to...

51:09

take charge of a lot of your design, you know?

51:13

It's, you know, he'll tackle the drop-down, hopefully, at some point. It's like, we've got the eye touch there. And so I think that it's interesting to talk a little bit about hardware and how that interacts just in the last couple of minutes with the overarching vision. So the overarching vision, in a way, you started at the beginning,

51:33

you talked about AI systems that will act a little bit like employees. I guess for people in their domestic lives, that's more like helpers. We don't generally have... We think of it as a super assistant. Like a super assistant. And so what is the relationship between that and the... the need to have a hardware device alongside.

51:59

I already have a hardware device. It's pretty good. I'm talking to it right now.

52:03

Yeah, I think it's more the opportunity. I think a lot of the, I mean, as we've said a few times, AI is going to touch every part of our lives and every part of our days in every part of the world. And that means, I think,

52:23

that there's an opportunity to reinvent and reimagine a lot of the services and the products that we use every day. And in some cases, there are a lot of products that I use every day that are great. They probably need to fundamentally change, and they should with AI. And if they're not,

52:41

they're not taking advantage of all these amazing new capabilities that we have, especially where those capabilities are going to be in 12 months, 24 months, 36 months. So I think there's an opportunity to reinvent and reimagine here. And that's true both on the software side and on the hardware side.

52:58

So, you know, we have some thoughts about how that might occur. Obviously, Johnny has thought deeply about this, and we're excited to see what we can build together. And I'm sure there will be lots of others building in the space. And that's one of the reasons that we have, like,

53:13

we put so much care and attention to our APIs and our developer platform. Because, you know, the world is not just open AI. The world, there's going to be incredible startups and incumbents and everybody else building really cool things using AI. And we'd like to power it in any case. You know,

53:31

some of these will be first party products that we build and some will be other products that others build that leverage our models. And, you know, both of those things are really important to us.

53:40

Yeah, I mean, I really, really, I mean, I hear that. I hear what you're saying as well, because I've already started to realize the limitations of the phone as the form factor for working with the models. You can't really put in a longish prompt to O3. I'm really reliant on talking to it.

54:00

And if I'm in a noisy place, that won't work. The idea of having an ambient intelligence around me, I always have. an AI model listening into my meetings, and I'm talking to them regularly to do my work. So you start to see the limitations of something that's got the power draw of the

54:15

phone and the size of the phone and does other things. So that will be a really exciting opportunity. And please sign me up for the alpha test well before GA. Done. We've got a couple of minutes. I just want to throw out some questions for you, very sort of quick fire.

54:34

How far behind are the top Chinese AI firms in core foundation model capability?

54:39

Not as far behind as they used to be. And I think as US AI labs, we need to be very cognizant of that. I think it's really important that the leading models, the models that we all use, are models that are built off of democratic principles, not authoritarian ones. And we take that really seriously.

55:02

Is there an AI app out there, whether it's in China or coming somewhere else, that's not built by OpenAI that you quite like and you like to use and play around

55:10

with? I mean, I think a lot of the video apps are super fun. I also find Waymo magical. That's my go-to example of the way AI is touching our lives. You know, again, like, self-driving was like two years off for 10 years and now suddenly it's here and it works and it's going to change a lot.

55:32

It's absolutely magical. You are a keen runner and I'm curious about whether you have a Garmin or a Suunto and what you would want from your exercise tracker that AI could bring that it isn't today.

55:47

Ooh, that's a good question. Um, actually I have, uh, an Apple watch that I mostly use. Um, and then if I'm doing like a hundred mile race or something, this doesn't quite have the battery. So I'll do a, I'll, I'll, I'll use a Garmin. Um, uh, what do I want?

56:03

I think actually one of the things that I would love is better coaching. Um, I just like a little bit. And I don't, I think the AI is totally capable of doing it. I think Strava has, you know, some things that they're working on around this. Um, And, uh, but I would love to see better,

56:21

better coaching and like, you know, AI, um, AI analyze, you know, workouts and, and things like that. So that I got the, I think it's possible to get the kind of analysis that you would get from like a professional coach today from an AI for most users. And I feel like that's the kind of thing that,

56:40

you know, five years from now, we're going to be like, oh yeah, can't even imagine when that didn't exist, but it's only sort of peeking through right now.

56:48

Just a little bit, but I do hear you. I think the possibility of having that personalized coaching would be quite sublime. So last question, when are you going to ship AGI?

57:00

We're working on it. Every day we get a little closer.

57:02

Every day, a little bit closer. I mean, when will we know? Will we know?

57:09

I think, look, I think it's one of those things that we talked about intelligence being multifaceted. There are already a bunch of places today where AI is way better than a human. And there are places where AI is like laughably worse than a human. But every, you know, every so, every like month or whatever,

57:29

when there's new models, the baseline creeps up. And more and more things, AI is becoming superhuman at more and more things. And at some point, it's going to be superhuman at substantially everything, and we're going to call it. But it doesn't happen all at once.

57:46

I think it's not like we go to bed one night and there's no AGI and we wake up in the morning and there's AGI. It's an incremental process of AI getting better and better at more and more things.

57:59

Well, with that thought, Kevin, you keep climbing that hill. Thank you so much this morning for giving us your time. It's great to have you. Thank you for having me. Cheers. Thank you. Bye-bye.
```