---
Summary: "KI verändert Softwareentwicklung: Automatisierung, Agenten, neue Rollenbilder."
Content Type: Podcast
Content Creator: Azeem Ashar, Thomas Dohmke (CEO GitHub)
Source: https://www.exponentialview.co/p/ai-and-code-what-comes-next
Date: 23.05.2025
tags:
  - AI
  - Softwareentwicklung
  - Automatisierung
  - Agenten
  - Entwicklerproduktivität
  - Cloud
  - GitHub
  - Copilot
  - Microsoft
  - Arbeitswelt
  - Produktivität
  - OpenSource
  - Coding
  - Content
  - Infrastruktur
---
---
## Wichtigste Aspekte

- **30%** des Codes in manchen Microsoft-Projekten werden bereits von **KI** geschrieben. Entwickler berichten teilweise von Verhältnissen wie **4:1** (KI- zu Menschencode).
- **GitHub Copilot** und ähnliche Tools unterstützen Entwickler in allen Phasen: Ideenfindung, Code-Generierung, Review, Testing.
- Die **Nutzung von Coding-Assistenztools** wächst mit **76 % pro Quartal** – schneller als alle anderen GenAI-Kategorien.
- Moderne Software besteht meist zu **90 % aus Open-Source-Bibliotheken**.
- Über **150 Millionen GitHub-Accounts**; Wachstumskurve Richtung **eine Milliarde Entwickler** weltweit.
- Beispiele: **Automatisierte Deployments** durch Pull Requests und Pipelines sind Standard, der kreative Anteil der Arbeit wächst.
- Trend zur **Personalisierung und Kurzlebigkeit** von Software: Programme werden für individuelle, temporäre Anwendungsfälle erstellt und wieder verworfen.
- Diskussion um **Komplexität und Kontrollverlust**: Code-Basen sind oft so groß, dass sie nicht mehr von Einzelpersonen vollständig überblickt werden können.
- Rolle von **Agenten** und KI: Unterstützung beim Auffinden, Verstehen und Anpassen von Code, Transformation bestehender Software.
- **Veränderung der Arbeitswelt:** Zukünftig können viele Aufgaben von jedem „User“ gelöst werden, klassische Softwareentwicklung verschiebt sich in Richtung Infrastruktur, Plattform, APIs.

## Thesen, Argumente, Erkenntnisse

### KI automatisiert und transformiert Softwareentwicklung  
- KI übernimmt einen steigenden Anteil an Code-Generierung und Routinearbeiten.
- Entwickler werden zunehmend zu Problemlösern und Systemarchitekten, nicht mehr nur „Codern“.
- Agenten und Co-Piloten helfen, den kreativen Flow-Zustand zu halten und repetitive Aufgaben zu automatisieren.

### Steigende Produktivität und Komplexität  
- Mehr Output (Code), höhere Qualität (durch automatisierte Tests und Reviews) und gesteigerte Kreativität sind eng miteinander verknüpft.
- Durch Automatisierung von Testing, Deployment und Dokumentation bleibt mehr Zeit für Innovation.
- Die zunehmende Komplexität und Verwendung von Open Source führt zu Kontrollverlust: Einzelne Entwickler können gesamte Systeme nicht mehr komplett überblicken.

### Veränderung der Nutzer- und Arbeitsrollen  
- Die Zahl der Menschen, die (unterstützt von KI) Software erstellen, steigt exponentiell.
- Personalisierte, kurzfristige Software-Lösungen werden zur Norm, Standard-Apps verlieren an Bedeutung.
- Softwareentwicklung wird zweigeteilt: Einerseits hochkomplexe, skalierbare Plattformen (Infrastruktur), andererseits individuelle Lösungen durch Agenten.
- Klassische Entwicklerrollen verschieben sich in Richtung Plattformbetreiber und Infrastrukturmanagement.

### Herausforderungen und Ausblick  
- Kontrollmechanismen wie Code-Reviews, Tests und Teamarbeit bleiben notwendig, auch bei zunehmender Automatisierung.
- Der Wandel zum „agentischen Web“ bedeutet, dass nicht mehr Menschen, sondern KI-Agenten zentrale Interaktionen übernehmen.
- Unternehmen müssen extrem agil bleiben, um Innovationstempo und technologische Komplexität zu bewältigen.
- Der „unendliche Spiel“-Charakter der Softwareentwicklung: Erfolg bedeutet ständige Weiterentwicklung und Anpassung.


---
### Transkript:

```
I think I will get us started now, Thomas. So here we go. I'll do my presenter setup. I'm Azim Azhar, and every Friday I have a long... I'll try that again. Sorry about that. I'm Azim Azhar, and every Friday I have a live conversation on what's happening with AI and our

0:20

economy and what it will mean for you. My guest today is Thomas Duncan. He is the CEO of GitHub. GitHub needs no introduction. It is the platform upon which nearly all modern software development happens, and software development is being revolutionized by artificial intelligence. Now, GitHub is part of Microsoft,

0:43

and recently Microsoft CEO Satya Nadella said about 30% of the code in some Microsoft projects is written by AI. This means that AI writes one line of code for every two lines of human rights. But that ratio is going to change as AI gets better.

1:01

And some developers have told me their ratio is closer to four AI to one human. When it reaches 100 AI lines of code for every one human line of code, Thomas, what is the developer actually going to be doing?

1:17

Yeah, it's a great question. I think Satya said 30%, between 20 and 30% of the code in our repositories was written by software. So it was a bit broader in how he framed it. I think the developer will do, do mostly what engineers actually do and how they define themselves, which is they're solving problems. They're implementing ideas.

1:45

They're taking the big idea you have in the morning. It's Friday 9 a.m. here. I'm sure many engineers here in the US look forward to a long weekend, but still have something that they want to get done. And they're trying to figure out how they do that. The work doesn't start with typing in your editor.

2:02

The work starts with reading up a GitHub issue or a specification or just taking what I have in my head and bringing it down into notes. And models play models and... systems like copilot play the first role here where you can brainstorm with them

2:18

and say hey you know i have this problem that i want to solve um you know very simple i want to build an app today give me some thoughts of how i can do that and you can kind of like do this software decomposition part first and take a big

2:30

problem break into smaller parts and i think that ultimately is what engineering means. And then you know where to stop with the decomposition, and now you can start coding. And in the past, you had to start at a very low level. Before we started the livestream, you showed me a very old computer.

2:45

And back then it was very hard. You had to go very low level. Today, most engineers actually already start on code written by others, right? They use open source libraries. They use open source app running systems. They have an editor that they're not building themselves and a debugger and a compiler and a container orchestration library

3:05

like Kubernetes and all these things, right? So we're already composing different pieces into software and we're moving up the abstraction level and AI will help us to achieve that. And then we will review the work of the AI to make sure it's secure and compliant and runs efficiently and hopefully returns some profit for the corporations or the

3:24

teams we're working for.

3:25

I love what you've done there because you've built us a bridge to the past. When people started to write code and I spoke to somebody this morning or yesterday morning when I was in Chicago who worked on medical records and he said the language they're written in is called mumps.

3:44

M-U-M-P-S, which I'd never heard of before and I'd gone off and researched. But, you know, in those early days, you started from a blank page, if it was in basic, 10, you know, print hello world. And what's happened over 35, 40 years is libraries, abstractions, reusable components. So an engineer is...

4:05

assembling things almost like Lego, but it's not as straightforward as a Lego. But there is something different about these AI tools, or so we're told by the numbers that come out on grand stages at developer days. How has your own experience as an engineer changed as you've started to use the co-pilot in GitHub?

4:28

Is there a behavior that you hadn't expected to take on?

4:32

I actually have some Legos in my hands and behind me too. In some ways, I actually think it is a bit like Lego, right? Because when you start working with Lego, you're not thinking about plastic pieces and forms to build bricks first before you assemble the bricks.

4:53

I think the thing that really changed through Copilot in my own coding projects, which are mostly hobby projects on weekends, is that I match faster back into the flow state. The challenge that most engineers have, and this is where Vibe coding comes, is that you have an idea and you want to build something on a Sunday morning.

5:15

And the first thing you did in the past is you started research and you maybe looked on GitHub. for some open source components or you looked on maybe something project already existed that you could fork and but before you knew it it was night and you had

5:30

maybe done a little bit you got a quick prototype done but you were nowhere near the thing you actually wanted to build and maybe you got to 10 or 5 and you realize that what you thought is easy to do is actually much more complex and That has dramatically changed through the use of open source,

5:48

through the cloud, through platforms like GitHub, Reddit, Stack Overflow, all these being available to you. Because when I started coding in the early 90s, it was books and magazines. And then on a Commodore 64, I had to build it all from scratch. So we are already at the point where we are taking pieces and we're composing software.

6:07

But now I open my editor and my project is there. And I can just ask Copilot, what's the next step? Or I can give agent mode the feature I want to build and say, hey, help me to build this feature. And then it looks through the files and it identifies where I have to make changes.

6:23

So I don't even have to figure that out myself. We're in the code base where I have to implement things. It runs command. And the cool thing when it runs command, it actually can look at the error message. and then see what is wrong on my system,

6:37

and it might have to install another library and things like that. So it keeps you more in that flow state instead of you switching back and forth between research mode and trying to make things work, and then things take forever to compile. In the meantime, you go and make a coffee or get distracted by Substack.

6:57

Well, if you think about the maybe three orthogonal dimensions about an engineer's output. There's quantity, there's quality, and there's creativity. Are they producing more lines of code? Are they producing better lines of code within a tighter set of guardrails? Or are they being more creative about the problem specification?

7:21

Which of those has most shifted when you look across the millions of people who've been using GitHub Copilot?

7:32

I think they, you know, to some degree have evenly shifted because they're all tied to each other. My creativity, you know, during the coding process is limited by the time that I have available and the energy that I have, you know, the amount of distraction I get. And oftentimes developers describe that as the magical flow state.

7:52

Like you're in, you're almost in a, you know, in the zone of building something. And as long as nobody distracts you, you really feel like you're getting a lot of things done. And then, you know, the moment comes where you finish the feature or you got the distraction and now

8:09

you're out of the zone and you have to find it back later. And I think co-pilot and agent mode keeps you in that zone of creativity and lets you refocus. Okay, I want to take this and implement it. Similarly, it helps you to review code.

8:23

So there's the Copilot code review agent where you can run your pull request through it and it gives you feedback on that. So you no longer have to wait for your team members, right? So that's not a creative process. That's more like a verification process and Copilot helps you with that work. It can write unit tests.

8:38

And I think most developers, if they're honest to themselves, and then certainly I can speak for myself, if I work on my own hobby projects, I write no tests whatsoever. And I don't file a pull request against myself either. right because it's like a all my code is obviously perfect haha but b it's like

8:54

that's not the fun part of the job the fun part is to implement something and i can see it appear in front of my in front of me on my screen and you have this i have the magic in my hands and i could create something with just with just code right

9:07

and so can i just demystify three terms you've said that may maybe need explanation for non-developers because this is a super relevant conversation about how work changes that we're having beyond coding and software development. So you said three things. One is unit tests. So roughly,

9:23

when a developer writes a component of code in order to know whether they've written the right thing, they should also write a test. If it passes the test, they've written the right thing. Unless, of course, they've specified the test wrongly. So that was one thing you described.

9:39

The other thing you talked about were the idea of pull requests. This is really about how you file each iteration of your code with a note of the work that you actually did so that you technically have an audit trail to work your

9:53

way back like Hansel and Gretel when they were meant to leave the sweet trail in the forest. And the other thing you said, which if people haven't worked with engineers, I think is so important, is the notion that an engineer gets into flow state. They become one with the code because what you're doing is you're taking the

10:16

amorphous complex world and you're framing it into logical deterministic code and it requires a class of focus that that I don't think you see in any other other activities now you're the you're the sort of developer advocate on this call is that a fair reflection of those three three ideas

10:37

I think you hit the head on the nail. Is that how you say it? You hit the head of the nail. Or the nail on the head, I think.

10:45

Either way, we're fine.

10:47

We're friends here. The hammer on the nail. No, but I think software development is a combination of creative work of art. something that's very similar to what an artist does. And it's also production, what Bill Gates famously called the software factory. And both of these things are combined.

11:07

And so part of the job of a developer is being creative, implementing something in software. And the other part is, working with a team of developers product managers designers to verify the product and that is both from a ui ux perspective like looking if the product actually does

11:23

and look like it was intended to be but also from a code quality perspective from a does the you know the the piece of software i produce does that align with what the rest of my team has been doing or is there now a conflict between those things so a lot of the time

11:37

that developers spending every day is actually on that production side of of of the of the creative process and often that is the more you know the more boring piece for many developers. And that's where automation is great because I actually want to spend more time in the creative part of it,

11:58

designing ultimately what I'm shipping to my customers and automate as much as I can on the production side. So to give one example, over the last... 10, maybe 20 years, almost all production deployment has been automated. So it used to be, you know, in the late nineties and early 2000s when the internet started,

12:17

you would have some files in your local machine and you would use a protocol like so-called FTP file transfer protocol and upload files to a box somewhere. Yes. Then replicate that process and maybe you had a script to automate that to some degree, but that was a very manual process. If something went wrong,

12:35

your page went down and then you had to figure out what did I do wrong or what server has a problem. Today, all you really do is you use this pull request that you described so eloquently where I submit my work for review by my team.

12:50

They review it, automated tests are running, verification is running, and then I'm click a button that says merge and it merges us into the main branch, the main line of our work. And then an automated process starts to deploy all of that into sometimes thousands, if not tens of thousands of virtual machines in the cloud, right?

13:09

And so that's one such example where we have automated the work of a software developer. So we have more time for the ever increasing complexity and demands and innovation on the creative side.

13:21

Absolutely. I mean, that's a great example where I think software developers are the first class of career where they start their day thinking, how can I automate away the things I did last week? And I've been around so long. You talked about continuous integration and deployment as opposed to manual deployment.

13:43

I remember the absolute excitement with a development team I was working with when we got something called Doxygen, which helped you create documentation. This is in the late 90s, because if there was one thing developers hated more than unit tests or more than deployment, it was writing docs. And Doxygen came out and helped you with that process.

14:05

So you've got this career class, right, where people have spent their time consistently thinking about how they automate what they do. I mean, I remember my sys admin from 10 or 12 years ago would spend about four days a week managing servers. And over the course of three months,

14:25

he got that down to a couple of hours a day using tools called Capistrano and Chef. I don't even know if these things still exist now. And so he started to do much more creative work. And it's one of the things I was wondering about, that desire to automate,

14:40

whether that is one of the reasons why tools like GitHub Copilot, but also Cursor and Windsurf and Replit and Lovable are growing so fast. If you look at the category of Gen.ai tools and the general models, you know, the Claws and the ChatGPTs are growing at about 20 to 22% every three months. No other category is

15:06

is growing remotely as fast as that, image generation, text generation, except the coding assistant tools, which are growing 76% quarter on quarter. I mean, still from a low base, a few million people every day logging in. I mean, to what extent is that just because software developers are, they like using software,

15:27

to what extent is it because they're bound to this idea of automating their jobs so they can get onto the interesting projects?

15:39

You know, we've talked about history already a little bit. And the way software developers have always worked is that they have tried to automate as much as they can of the workflow, but also they have moved up what I call the abstraction ladder. And 50, 60 years ago, they were still punch cards.

15:57

They would punch holes into a card because that basically a hole was transistor open and not a hole was transistor closed or the other way around. And then microprocessors came when Microsoft started in 1975, there was a very popular, it's funny to say these days,

16:16

because it was like maybe thousands of devices in a very small scene of people, but where all of a sudden you could program the computer in a programming language. And so the first Microsoft product was BASIC and BASIC, what BASIC did is it abstracted the instruction set of the chip which is ultimately numbers in hexadecimal form,

16:42

abstracted that into something that is human readable and is pseudo English, right? Like if you look at almost all the popular programming languages by Python, basic, Rust, they all have English keywords. And the reason for that is that obviously our thoughts are expressed in the language that we speak, not in computer instruction sets.

17:07

And so we abstracted the complexity of the chip into something that is closer to the ideas that we have, the features. but there was still a huge gap between the description and instruction set. And over the years with open source components and higher programming languages and things like that, we moved closer,

17:25

but we never got really there until GPT-3 came. And when OpenAI launched GPT-3 in 2020, they created a fine-tuned version of that called Codex, fine-tuned on open source code that for the first time allowed developers to describe their ideas in English and then later in German and almost any major human language.

17:48

And then the model generated the code for me. And in 2020, that meant I could say, give me a method to determine prime numbers or do sorting algorithms. And if the listeners have gone to university and did computer science, they know that you have to learn all these different sorting algorithms, quicksort and bubble sort and whatnot.

18:07

And then you never needed that again, because ever since you started your career in a company, you just use some library and do array.sort. And so we've always moved up that ladder, but all of a sudden with AI, we were able to get so much closer to how we're actually thinking,

18:25

the language and the descriptions that we're thinking in. That's number one of why the adoption, the diffusion of these tools has been so fast in software development because it finally got us to the step where we always wanted to be.

18:40

This arc that you described, where we go from assembler language, which is, I recommend people take a look at some if they haven't. It's pretty indecipherable. through to higher more sort of English natural language friendly languages like Python and Rust makes a great deal of sense.

19:01

And then of course you move in towards open source and open source has these highly inspectable bazaars. They're not these uninterpretable cathedrals. You can put your library up and other people can look at it and people can fork it. They can run their tests. There's a sense of trust in what's going on.

19:22

But there is an argument that says, as we move to AI writing 400 lines of code for every line I write, that it doesn't become inspectable. I mean, a human couldn't inspect the source code in a modern jet plane, for example. No single human could. So we... Isn't there a case that we've gone over the hill,

19:45

over that point where the languages were high level enough, abstracted enough that we could understand them, to a point where we're going to be creating so much code so rapidly that it'll be less inspectable for the human?

20:01

I believe you're already past that point. With or without AI, we passed that point a few years ago when it became clear that the majority of projects, commercial or not, are based on 90%-ish, plus or minus of open source libraries, open source systems, a few. You look at what runs on a platform like Substack today,

20:24

it's not only the product itself, it's all the open source libraries. And keep in mind, those open source libraries are maintained by millions of developers around the world that are not part of the organization that sells the product, that do not follow a work schedule, that do not the same trainings.

20:41

that you know might decide on a sunday night uh to push an update to the library and so now all of a sudden you effectively gave commit access to those to those people because they're part of your stack all the way down to the operating system

20:54

that almost nobody builds themselves and even if you look into the you know linux windows or other mac os operating systems they're incredibly complex that a single person it's very rare that a single person can navigate that whole code base, right? So what do companies do? They divide and conquer and they assign subsystems to individual teams.

21:15

And that's in some ways the funny thing about software development is that What you learn in school and university is the basics. And then what you really learn is the craft through your journey. When you come into a company, you realize you almost never get to start a new project and start from scratch.

21:34

You almost always get to maintain somebody else's work. That might be, you know, there's still many financial services companies that run on COBOL, which is a very old programming language that was invented when Eisenhower was the president in the United States. Runs on mainframes, which is technology that was, you know, the state of the art in 1975.

21:57

That still runs, right? And somebody has to maintain that. So we are... I think what you're saying is absolutely true. We're already at the state where a single person often cannot explain all the different parts of the system. And so AI actually gets us closer to that state again, because now you can just ask Copilot,

22:19

where in my code base is the feature implemented? What does this method do? What does that method in COBOL or the struct looks like in a more modern language like Java or Python? And so you can do these transformations. You have an agent, a coding agent that's always available to you,

22:38

And this week at our build conference here in Seattle, we announced the coding agent and co-pilot where you take an issue, literally like a human language description, and the agent does all the work in the background and submits a pull request. Now, I get that pull request. I still need to understand what that actually does, right?

22:55

Like, how do I decide whether I can merge this or not? Of course, I can YOLO it, right? I can just, you know, only live once.

23:03

I mean, how do you do that, right? How do you... give some assurance to possibly a complex task that an agent has worked on for 45 minutes or an hour and make sure it's right. And, you know, how does the discipline, what used to happen, I guess, in engineering teams was that,

23:20

you might show your commits to your neighbor who's a peer of yours and say, this is how I approach it. They might ask you the questions. And maybe once a week, your team manager might sit down with you and ask you to walk through some of the

23:34

things you've done as a measure or beyond whether you've passed the unit tests. But How does that team now work where you fired lots of things off to coding agents to go and build? Where do you get the understanding, the assurance from?

23:52

It starts with a planning process, you know, the process of describing what you actually want to implement and the key new skill that engineers, product managers, designer, whoever's using, you know, this orchestra of agents that helps us all day, you will learn and internalize

24:12

what is the right level of description that the agent needs to do actually what I want it to be. Now, of course you can, when you try out an agent like this, you can just give it a very abstract task and see what it does. And very quickly we'll find out, and you mentioned earlier image generators.

24:28

I think image generator is actually the perfect abstraction of that concept, right? Like the first time you used an image generator and you told it you want to render an image of puppies, or a computer on a meadow or something like that, right? You most likely didn't get exactly what you wanted.

24:44

You got something that was close to the description and then you knew that, okay, I write another prompt and you try to figure out how do I change my prompt to now get closer to the image I want to get to. And the same is true for coding agents, right? You will try it out, you'll see, okay,

25:00

it wrote something, but that's actually not what I wanted or it doesn't align with our standards here at GitHub. And so then you go back to your description and adjust your prompt. And as you learn that skill, you're going to get better on describing exactly the task that the coding agent can take, run 45 minutes,

25:18

submit a pull request, you review the code, and you're like, yep, this actually looks good and it does exactly what I want. And you will be wrong at times. You will be either too... far away and then you will have to work with the agent and understand, you know, how do I get it now to the point?

25:33

And I think what would be crucial here is that developers will want to just take the code on your local machine, on their local machine and modify it because there's always going to be a moment where you're like, this is three lines of code.

25:44

I know exactly what I'm doing instead of me trying to figure out how to tell the agent to change those three lines of code i just change it myself so we will switch between the natural language layer and the the coding layer all the time but let me

25:58

let me ask you about how how this changes as the software changes you know you've described that a lot of developers in the world are you know they're not working on the next tick tock they're actually maintaining a customer database for a shoe factory And they have to go in and do that work.

26:16

And what you're doing is you're taking the technologies of tomorrow, which is AI, pointing it at the systems of yesterday and maintaining them. Everything needs maintenance. But of course, we're going to start to build new things. And the word agent, of course, is in vogue.

26:33

And software agents from you and Cursor and Record and so on are all part of this system. But the nature of the software that companies are going to ask for is also going to change. I would posit that if you're a big company and you've got a system of record like... a NetSuite or an SAP,

26:58

what you probably want to do because you've been basically stuck in this stack is start to build a layer of agents that do the things that you need for your customers, your suppliers, your team without having to build traditional software, just talk to them through an API or through browser use, which is getting better and better,

27:22

and abstract away those old complex, almost kidnapper style bits of software. And move to a new architecture, which is ultimately about building more agents that work with each other. I mean, is that a reasonable direction of travel? Or do you think I've simplified it to an absurdity there?

27:47

No. I would actually follow your logic, but even layer it a little bit. You mentioned a number of these agents. And so let's say you and I want to build a web page where we sell shoes, right? You can just go to any of these agents and have it build the web page for you,

28:04

and it can even deploy it. And you never have to look at the code of that web page, right? Because that used to be called low code or no code. And a lot of these very simple things you can build without ever looking at the code.

28:17

Now our shoe empire goes and now we have a full e-commerce store and we need a backend and a warehouse. Now, what started simple no longer scales and all of a sudden, a million buyers come and the webpage is down on Black Friday. How do you figure out to make that actually work.

28:34

Now you need to go into what is actually the part of engineering, which is not building this quick webpage, hacking it together is what we used to call it, but figuring out how do I make the scale? How do I have the capacity on Black Friday?

28:46

But don't waste a lot of money because servers cost money and that ruins the margin of our business when there is no demand. And so we have to build an abstraction layer in between, for example, for all the shoot pages to have the same design system, design components. And so when we decide, okay,

29:07

we're five years into our business and our brand color is no longer purple, but pink. that we can just change all the design at once instead of having the agent go to every single page and modify that again, right? So we got to build a stack, an engineering stack, a platform stack that resembles our business.

29:25

Another example is at GitHub, we have a product called GitHub Actions, which is our continuous integration deployment service. And we are looking into how can we get that from 99.9% uptime to 99.99, so-called four nines uptime. That's not something you can just go and ask the agent. This is an engineering problem that you need to solve.

29:47

That is very similar, I think, from a complexity perspective, if you're the mayor of a city and you promise everybody you're making public transport better. That sounds simple when you're promising it during the election. And it's much harder when you're actually elected. And now we have to figure out how do I change the city?

30:03

How do I get the permits? How do I build? Where's the funding coming from? And I think that is where you're always going to have humans. humans that use agents and combine different agents, but you've got to know at which point in your day-to-day process, in your engineering process, you're using these agents for what purpose?

30:24

Okay, so I think what you're saying there at that point is that it's one thing to write small chunks of code that can do a function or a personal app, but embedded in what is effectively a complex system of enterprise software with thousands of functions and services where that can be quite brittle because one is very

30:47

sensitive to how quickly it gets a response. And over the years, you've built in cues and other mechanisms to make sure the whole thing works. That is almost an undocumented, implicit knowledge that the senior engineers have of a system And your contention is it'll take a while for AI systems to get there.

31:10

So we're going to see two trends, right? Today, you're buying software, SaaS services, platforms like Substack, because it's cheaper for you to spend a small amount of dollars every month on those platforms instead of orbiting it yourself. If building it yourself with an agent becomes so simple that you can just do that in a couple of minutes,

31:30

you will stop paying for these SaaS services.

31:33

Right.

31:34

you know, we will see a commoditization of software that is so simple that recreating that on the fly will replace those SaaS services. And one such example is Manus, one of the tools that became very popular in recent weeks. And I met with the founders a couple of weeks ago and they showed me how they were

31:55

looking for an office in Tokyo And so instead of just going to a real estate page and kind of creating a note sheet of what is interesting, they had the agent create a map of all the available offices just for them, right? So it's personal software. It only serves that one purpose.

32:12

Once they found an office, they can throw that away. And whenever they need to find bigger space and whatnot, they recreate that software, right? So that level of software effectively has lost most of its value. And it's only because the creation is so cheap. But at the same time,

32:29

everybody using agents will create so much more complex software because they can now, with the same skills and the same capabilities, add features to their platforms like GitHub at an accelerated pace. And so hopefully, you're still finding value in buying these platforms and paying for the service

32:49

because the complexity there is increasing as much as the simplicity commoditizes the more simple applications.

32:57

Yeah, I mean, it's very true. I have a really personal example. So my physio gave me a program for a month, and I took the program and I threw it into one of these vibe coding platforms. These are products you can go to. They've got a prompt. You type in a description, it generates working code.

33:18

And it generated me a working web app called Build Back Better, which I thought was a great name for a back... program. And it's just for the four weeks that I've been using and tracking and doing the work. And I didn't go off and buy something. I didn't find something that didn't quite fit my needs.

33:38

So you start to see things like that emerge quite quickly. And you yourself talked about a world of a billion developers, right? So we currently have about 50 million developers. And you said, well, you can envisage this world of a billion. But that feels like a phase change, right? So what are a billion developers doing?

34:02

They're not debugging SAP, right? Or COBOL or Dibol or in an IBM 370, right? So what does that actually mean for there to be a billion developers?

34:13

we already have um 150 million accounts on github now i'm sure there's you know some duplicate accounts and some bots and whatnot um but we are on a path um if you look back where github came from 17 uh years ago when it when it launched in april

34:29

20 2008 uh now we're at 150 million you can just continue that exponential curve um and predict that by you know 2030 or so we're going to be at uh at a billion and From my perspective, the most important thing about this number is that we have way more than a billion computer users.

34:50

In fact, we have more than a billion smartphone users on the different platforms. And a lot of that smartphone usage today is consumption. You're downloading an app or you're just opening a browser You're watching videos and reading text. And that actually is different to what computers were 50 years ago when you bought your first, well,

35:14

PC wasn't around, but like microcomputer. And where you started with creating software, you had a basic prompt on a Commodore 64, and so you had to learn a little bit of coding. And I think we're going back to that, that every consumer is also being empowered to be a creator,

35:31

just like you're using your camera already to create on these phones and your email app and whatnot. And I think that's crucial that it's important for us that these devices let us create whatever we want to create. And the programming language is not in the way of that.

35:48

Sorry, I mean, I love that picture. So let's play around with what that might look like. I mean, the tools are pretty good today. I don't think they're quite there for a billion people. You still, you know, the agents still make mistakes and you need to know a little bit about CSS styling

36:04

and other types of questions when you look at the preview. But it is really... you know, enlivening, in fact. And I wrote my first code for the first time since 2012. I had been banned by my engineering team from writing any more code back then. And I had to set up a new GitHub account.

36:26

And this code does one thing for me. It's a little extension on my browser that allows me to count the number of words I've highlighted. And there are lots of word count extensions in the Chrome store, but they all have other features I don't want. And this one I've been able to run.

36:43

I just got Claude to write it for me. chat GPT to check there were no security problems and it's been amazing because I haven't been able to do that for 15 years but you know you work with you work with developers all the time that's been your life so what happens when a billion of us

37:00

are able to to do that right how are we interacting with our with our computers and with each other

37:08

So that's the other side I see is, you know, we have a billion, well, we have more than a billion, way more than a billion people that learn math in school and that learn reading and writing in school and they have arts and sciences and physics and maths and all that.

37:23

But most folks then after school, most students after they leave school pursue one career path. And just because they had, you know, math in school, that doesn't mean they don't become a mathematician. Now that might also be because that's, you know something where you don't make a lot of money as a mathematician but you

37:41

get the idea right we're teaching our kids the fundamental skills of life and i think computer science is part of these skills so that's number one like we need actually every human on this planet to understand the basics of these devices that

37:56

are so dominating our lives and it will only get worse from here um you know the

38:01

future will get better perhaps depending on your perspective

38:05

Sorry, that was you, the optimist, and me, the German realist. But worse in the sense of we're going to have software and computers everywhere in our lives, self-driving cars, and our alarm is a software, and our house is controlled by software, and travel is controlled by software, all that.

38:25

And so then there's the intersection of you can do it because you have learned it or you want to make that your career. You become a professional software developer. And I think that that's a Venn diagram that will never be perfect because not everybody in this world wants to be a software developer.

38:42

You know, people want to be outside. People want to be in the kitchen. They're becoming a chef. They want to build houses and whatnot. But to take your example now, you know, the builder that works on your house, you know, to build your new deck or whatever, right?

38:58

Will now probably build software for your project that is between you and him or them and that, you know, the crew. And that software will be there for the part of the project. So you don't have to create an account for some platform. You don't have to accept the terms.

39:15

And maybe there's still a billing platform and credit card stuff. And because that will always be simpler through something that's standardized. But you're going to have a personalized piece of software, and I think we're going to rethink these devices, and you see some folks in the industry already doing that,

39:31

where a lot of that is more like an agentic interface that is highly custom for you instead of having a grid of icons. Right. You know what you've described, though?

39:42

that um you know there was that no code movement some years ago which uh for people who aren't developers meant that you could build applications without just by joining blocks together and actually when my house was renovated i did in fact

39:56

build an app for it uh so when you take the house over from the builder you have to go around and find all the snagging right where did the paint not finish where's the a door not closing properly. So I built a little app using something called Airtable, and you could take photos of it, of the thing,

40:13

and it would get dropped into this database, and then we printed it out and gave it to the builder. And it was an incredible feeling back then to just produce this thing. It was time-limited. It came and it went. But the thing is, of course,

40:28

a lot of the 100 million people who are on GitHub and the 50 million professional software developers make their money by writing software that is built and used by many, many people. And we pay $50 for it or $1,000 for it. So in this world of a billion developers, don't you naturally suppress the

40:49

the wages in the coding community? Don't you dampen down the number of formal roles that are there? Because I'm not buying, downloading an app on the App Store now because I can just quickly whip up the thing I need.

41:05

You're not downloading an app from the app store, but you're building your personal applications that are connecting to what we call the agentic web, you know, servers, APIs, application programming interfaces, you know, information stores, databases, payment gateways, all these, the models itself, you know, the GPU clusters and around the world to actually enable all these scenarios.

41:34

So there's going to be the infrastructure that enables you to build that app. Of course, you're still going to buy some device. And as a good nerd, you're buying a new device way too often, way more often than you actually need a new device. And that device runs an operating system and has connectivity that connects to that

41:55

agentic web backend. And I think... what will go uh away in the sense that nothing actually ever goes away but will fade more into the background is this notion that everything has a highly um branded web page like take take take you know an example like i'm going to paris uh

42:14

in a few weeks and and today when i booked this trip i going out to to a web page to book my plane ticket or train ticket and book a hotel on a different web page and I book a rental car or driver. And so three times I've entered the same from to date and have accommodated for

42:32

when I arrive and when I leave and looked at my calendar 15 times. Why can I just not just go into my agent and say, hey, I'm going to Paris. This is the, and you describe in natural language what you would actually describe to the human travel agent.

42:45

And then maybe it builds even a web page for the trip. And so you have all your bookmarks there and all your images, highly personalized. But all these pieces, all these features connect to infrastructure and to processing, to ultimately whoever is selling you the service.

42:59

Because it's not like you're having an agent that builds an airplane that flies to Paris. Although that would be kind of cool if that existed. Yeah. Yeah. Please go ahead. Go ahead. the world that we as humans enjoy is still mostly physical. And it's mostly based on services provided by others.

43:24

And even if you like making your own food at home, you still have to buy groceries because you're not growing all these in the garden. But even if you grow all of these in the garden, then you have to buy, then you have a good customer of Home Depot to get all the gardening materials and the tools,

43:38

right? And so the same is true for software. There's always going to be some part of the stack that the professional software developer companies like Microsoft, Google, and so on to provide to you. What is really changing is the way you engage with that stack. And instead of taking off the shelf apps, you're going to have personalized.

44:01

The misconceptions a little bit that we're just replacing existing apps on our home screen with new apps that we built for ourselves. I think it's much more on the fly that you're engaging with your agent. Tony Stark in Iron Man has Jarvis and effectively engages with Jarvis, his computer, only through natural language.

44:17

But every time he needs something, it has this hollow image screen in front of him and he can see how he can build a time machine. And so I think this is how I'm thinking about agents helping us to build software for your house, you know, for my Paris trip,

44:33

but it's built on top of a stack that's provided by a technology industry. And I think that technology industry will sit on so much more complexity and so much more scale because now a billion people generate software that connects with those APIs at any, it's almost like we are enabling a world where the humanity

44:54

constantly runs the distributed denial of service DDoS attack against the whole tech industry, right? And so the scale that you have to build, and that's why companies like NVIDIA, you know, have been thriving so much over recent years. The scale that you have to build is magnitudes larger than what we have today.

45:11

What you're describing there is a fundamental shift of the web, right? You can't call it a re-architecting because there's no architect. It's going to come bit by bit, step at a time, where the web has really been built built for people. We've had APIs on the web that allow computers to talk directly to particular resources.

45:36

But essentially, the starting point of the web actually is the mobile view, right? Then it's the web view. And then you think about the API. But those first two things are not really useful for agents at all, right? They don't need to see. And in fact, what you're starting to see emerging from the startup community are many,

45:58

many tools that effectively agentify web pages. So you take these beautifully designed web pages for humans, a module runs over them in order to reliably allow an agent to programmatically get information or put information into it. And at some sense, and this may have been Satya who said this, but it may have been somebody else,

46:18

that essentially software is a user interface stuck on top of a CRUD system, creates, read, update, delete, database. And in a way... What you're describing is that sort of thing where I might be the person who has the really great data on food composition,

46:39

and you might be the person who has great data on room availability in European capital city hotels, and the agents will come in and query that information. to then build the experience that the end user has. It's a fundamental shift from the web because the web has been largely paid for by

47:02

human attention on human constructed pages or pages constructed for humans. So just, you know, you're a master of change management because you've worked with the software industry for a long time. So talk us through the steps from this human oriented web funded by human eyeballs to an agentic web,

47:24

which is about this intelligence autonomous infrastructure that my agent or agents can interact with to build my experience.

47:33

the most crucial thing especially as my in my in my role as ceo of github is you got to meet you know the customer for us that's software developers you got to meet them where they are you got to bring the products where they're already doing you

47:47

know their work uh it is much harder to convince you you know to change everything in your in your in your on your computer or in your life in your house uh because i to convince you of that new future and ultimately sell you that future instead of

48:02

telling you here install this into you know your existing environment and you get ai features and you know when we launched copilot in 2022 we didn't we didn't even focus on this there wasn't generative ai it wasn't a hype And so we mentioned, we called it the AI pair programmer,

48:17

but ultimately it was positioned as something that makes your coding experience a little bit better. And it was very much in the background in the IDE, which is the editor. And when you typed it, it gave you a suggestion. The flip side of that is that you gotta have a vision.

48:38

We often call this the North Star of what that future looks like. And the challenge specific with AI is that there's two camps. There's the one that believes the artificial super intelligence or general intelligence is coming. And that's just replacing everything as we know it because it's going to be so

48:56

intelligent that it doesn't really make sense to even write, have an editor anymore and see code. And maybe that future is coming. I don't know. But we certainly don't know how far away that is. And that's tricky if you're running a business today.

49:13

and the other side of that is that you know you build you to gradually get closer to that future but every step of the way you're making smaller innovations to what you believe is realistically achievable in the next in the next three to five years

49:27

and even that is moving so fast that you're going to be off and so in software development you know we've been calling this agile development for quite a while. Where we are today in technology means you have to be incredibly agile. A company like GitHub or Microsoft needs to be as agile as a 10-person startup.

49:45

And that is quite hard because we're running a big ship at the speed of a really small boat that can turn very small circles. And so I think finding That every single day, finding the energy, finding the motivation, finding the steps that we need to take to have this agility, even though we are running this large ship,

50:07

that is what is required in this world of AI. And let me give you one last metaphor, because we talked a lot about these. We have seen self-driving cars. Whoever has been to San Francisco has hopefully been in a way mode to see what that is like. Yeah, amazing. Yeah.

50:23

And today, most American houses in the suburbs have a two car garage. And so, you know, a significant amount of space on our lot is taken by that garage. Now I could already start building houses without garages in the aspiration that soon enough, you know,

50:41

way more and similar cars will be everywhere and i don't need a garage anymore i can have a much bigger lego room in my house but the reality is we're not at that point yet and so i can't do that yet so i can have that dream and that vision but

50:55

in the meantime i still have to build garages and and and work work our way into that future that we are seeing and i think that's the the fundamental balancing those two the the vision you know, the aspiration of where the world is going with where we are today in reality,

51:10

and then making incremental changes at a very fast pace. That is what allows us to stay ahead in the world in the age of age.

51:19

I'm going to pick up on that in a second. I want to think about something that you said about your customers, because you're close to your customers who are the software developers, and GitHub hosts millions of pieces of software, many of which are publicly accessible.

51:31

And so, you know, what a lot of investors do, I remember doing this myself, repositories are growing really quickly and you get in touch with the guy who's written them and the woman who's written them to see if they'll accept your money. And I remember a year or so ago that Agent GPT,

51:48

which was this framework for building agents using GPT-4, was getting all the stars on GitHub, which is like, I guess it's like a Tinder swipe right, right? Lots of those swipes happening on it. Really, really popular. And it allowed people to say, well, that's where the smartest developers are kind of veering towards.

52:06

So looking at what you're seeing across GitHub, right, what are the little hotspots that are going to be really exciting in the next six months and a year because you're seeing the smartest of your developers star, clone, fork, repos? You know, tomorrow,

52:27

this weekend is the Formula One race in Monaco and Saturday is qualifying and Sunday is the race. And what you described is you look at what the qualifying result is and you assume that that's also the result of the race. Now, that may be true for some races where you can't overtake,

52:43

although now they do two mandatory pit stops. We will see what that's like. But it describes a bit of what, you know, the world that you see is changing. There's a lot of great ideas out there. There's a lot of projects that have really steep adoption curves. That doesn't necessarily mean that they're winning and vice versa,

53:02

you can have a winner that comes from behind and was in the shadows for a while. This goes back to what I said earlier. The crucial piece is that you've got to keep it up. In software, there's no stable state. The world is always changing. What is the new shit today is going to be outdated tomorrow.

53:25

And we see this in AI even faster than we've ever seen it before. And so it means no matter what project you're looking at, you've got to see, OK, so what are they doing next? And how often can they keep up with the work?

53:37

And that is as true in the enterprise or in the commercial software space where you keep your source code closed than it is in the open source space. And I think survival, The best way I can describe this is they're all playing Minecraft. There is no ultimate win.

53:55

There's little mini-wins that you have, but you're playing an infinite game. You're playing an infinite game, and survival and staying on top of it, that is actually the skill for software engineers and the groups that they're forming to build companies.

54:14

I mean, I think Steve Jobs said that the computer is the bicycle for the mind. If the computer is the bicycle for the mind, software, I suppose, are the unending roadways and hills and places that you can travel. Thank you for your time. One last question for you. I know you talked about Minecraft. You love Lego.

54:31

If we could bring these two things together, Lego and AI, what would be your fantasy agent? What would you want to merge those loves of your life?

54:44

The magical thing I think for every Lego enthusiast is that I can give it all my unsorted Legos and it perfectly sorts them by size and color into the container store bins that I have upstairs. There is an app on smartphones that does that to a smaller degree, but I would love kind of like a little machine,

55:07

you know, maybe it's the size of a dishwasher and you just put all the Legos on top of it and it sorts them all into the bins. And so you don't have to do that yourself. That's the nature, I think, especially for parents at home.

55:20

Lego, the magic of Lego is that you can take it apart and reassemble it in any possible way. But that also means you're creating entropy. The Lego room is always going to have entropy. And then bringing the entropy back into order is the... And the funny thing is, if you take that into software,

55:42

that's exactly the same for code, right? Code also has entropy, like code bases always get worse. Even if they're stable, then they get worse because the world around the code base is changing new libraries, new operating system and so on. So keeping the code organized and clean and healthy and scalable,

55:59

that is what engineers are looking into with these agents. And so they can then use their time, their creative time to build something amazing.

56:07

Thomas, on that chaotic note, I'll also get you a humanoid robot to load your Lego sorting machine at some point. Thank you for all of your time this morning. Thank you so much for having me. Cheers. Bye-bye.
```