[00:00:00] Beatrice Erkers: Welcome to the Existential Hope podcast, where we dive deep into the minds and visions of some of the world's most forward thinking individuals. I'm your host, Beatrice Erkers, and I co-host this podcast along with Allison Duettmann and today we're really diving into the world of AI and AI safety with Dr. Roman Yampolskiy. Roman is a leading computer scientist and he's at the University of Louisville. His work spans everything from behavioral biometrics, the security of cyber worlds, and most critically maybe, the safety of artificial intelligence. He has over a hundred publications to his name, including pivotal books on AI safety, and he really is at the forefront of understanding and mitigating the risks posed by advanced artificial intelligence.

[00:00:44] Beatrice Erkers: Before we dive into our conversation with Roman, a quick reminder to sign up for our newsletter. It's the best way to stay connected with the Existential Hope community and keep up with the latest episodes, insights, and updates. Also, make sure to visit existential hope . com. After the episode there, you'll find a full transcript of our conversation, a curated list of resources for further exploration, and an exclusive art piece inspired by our discussion with Roman.

Meet Dr. Roman Yampolskiy

[00:01:09] Beatrice Erkers: Now without further ado, let's welcome Dr. Roman Yampolskiy to the Existential Hope Podcast.

[00:01:18] Allison Duettmann: Hi everyone. Welcome to the Existential Hope podcast. Really excited to have Roman Yampolskiy here. Roman is a very dear collaborator at Foresight. We've followed your work for quite some time and I think Christine almost longer or like Christine - Foresight's co-founder longer than I have even had the chance to follow it along, since I joined Foresight about 10 years ago.

[00:01:38] Allison Duettmann: Just a little bit to your background and I'm sure that you'll fill us in a little bit more. You are a tenured associate professor at the University of Louisville, and you focused on the kind of intersection between security and AI, I think in really useful ways and have been drumming that bell for a really long time, since way before it was cool.

[00:01:53] Allison Duettmann: So it's really fun to have you on now and this podcast. You've also been a Foresight fellow alum, and we have actually in the past co edited this special issue on super intelligence coordination strategy together. But I think you're really well known for your work at the intersection of AI and security in particular, and really putting your finger on where it's hard and why controlling AI systems is so difficult.

Diving into AI Safety and Security

[00:02:14] Allison Duettmann: And so I really hope to deep dive into that in the introduction, but maybe bring us up to speed a little bit on what you are working on from your perspective, and then we can pull on some threads.

[00:02:23] Roman Yampolskiy: Thanks for inviting me to your podcast and for this wonderful introduction. I just had a book released, which kind of summarizes my ideas in this space, - what possibilities in AI safety, can we actually control superintelligent machines? Can we understand how they work? Predict what they will do? Explain specific decisions they make, not just in general, but a step by step process they go through to arrive at those decisions.

[00:02:53] Roman Yampolskiy: And so far, I haven't seen too many solutions. I found many ways not to build safe superintelligence, but hopefully I am wrong and we'll discover a lot of reasons for existential hope.

[00:03:05] Allison Duettmann: Well, shall we just dive a little bit more into these specific topics? So first and foremost, can you maybe just bring us up to speed? Why do you think the relationship between security and AI is perhaps one that is underexplored these days?

[00:03:16] Roman Yampolskiy: So one of the ways AI could be very dangerous is malevolent use, right? It's not that you build a very evil AI, it's just somebody got access to it illegally or you open sourced it and the bad guys, terrorists, crazy psychopaths, governments, military, whoever is using it in a way you are not happy about.

[00:03:38] Roman Yampolskiy: So if you open sourced it, it's on you, but if you did everything you can to protect the code and they still managed to hack it that's a security issue, right? Standard cyber security. You want to protect the code, protect weights, protect any secret source you have in developing this very capable system. Safety on the other hand is about safety from the agent itself, safety of the AI as an agent, which may have intentions and goals different from wherever trained and designed it.

[00:04:08] Roman Yampolskiy: So I think you need both. You need safety and security. Otherwise it's just not enough. Even if you are successful at solving one of the two problems, the second one will get you.

Challenges in Controlling Superintelligent AI

[00:04:19] Allison Duettmann: Yeah, I think you're making this argument of alignment being almost like a subset of safety and control issues. Could you explain a little bit more, - what you mean by that, and especially on the control aspect, perhaps why you think that one's really hard?

[00:04:30] Roman Yampolskiy: Yeah, so for about a decade we had these naming wars. What do we even call this problem? We started in the sixties and seventies with just ethics, computer ethics of computation.

[00:04:41] Roman Yampolskiy: Then I think Zer proposed friendly ai. Since then, we had control problem. We had human compatible. I proposed AI safety, but we all understand what we're working on. Whatever the name is, we want to create AI we will not regret creating. But the way I see it you have safety as the general name for the field. We want safe AI. And then people propose specific methods for getting there. So value alignment to me is one specific method you can use to assure that the system behaves as you would like it to behave. But a lot of people think alignment is the whole field. That's what we're working on.

[00:05:25] Allison Duettmann: Yeah, it's so interesting. Sometimes when I try to break it down, I try to break it down into alignment as consisting of, just like technical alignment. And then also we need to eventually figure out like, what do we want to align to? Then the security aspects of like really securing that, like eventually AI systems that we're building are built on secure foundations so that if we could align them to the values that we would want, we could do so reliably and securely rather than them, like getting stolen or like breaking out.

[00:05:50] Allison Duettmann: And then the last one is assuming that all of these are hard. We need kind of coordination and cooperation along the way. And that's more like international cooperation, AI governance kind of field. But yeah, it's really interesting how you slice the different fields and how they all spawn out and collaborate really across each other now.

[00:06:06] Allison Duettmann: But you are also making this argument that it may actually be really quite difficult to like, really make sure that we could control advanced AI systems, like even just like on a pretty foundational level. Could you explain a little bit more about that and what do you mean by this?

[00:06:20] Roman Yampolskiy: I think everyone agrees it's difficult. No one's saying like I can do it in five minutes. Just give me a little more funding.

[00:06:27] Roman Yampolskiy: I'm arguing that it's impossible to indefinitely control superintelligent systems. We can definitely control narrow AI systems we have today. We can make systems which are close to human capabilities safer in proportion to how much resources we have spent, computational resources, human resources. But forever controlling superintelligence is like building a perpetual motion machine. Maybe you are successful at the next generation. Maybe GPT 5 you, you are doing well with, but it will continue learning, continue getting better, smarter, self improving, modifying this code.

[00:07:06] Roman Yampolskiy: So really the problem is, can you make it safe for version five, six, seven? Up to infinity, while still dealing with security, malevolent actors, insider threats, and if that's not difficult enough for you, then we talk about value alignment problem, we don't really agree on any other definitions. As you said whose values are we aligning with?

[00:07:32] Roman Yampolskiy: There are 8 billion agents –  that's excluding all the animals and whatnot, and humans don't agree on much. That's why we failed to solve ethics for millennia. So maybe you can get a system to align with one agent, but it's also that agent at a specific point in time. What I want today and what I wanted 20 years ago. It's not aligned even internally, you have inner alignment problems, you have all these issues, but let's say we solved it and you actually know what you want.

[00:08:06] Roman Yampolskiy: We still have no idea how to encode those concepts in a formal sense in a programming language. We don't know how to make sure that the system we build will follow through on that, not just today. It may be perfectly aligned today, but there is always possibility that it will learn some new information and turn on you.

[00:08:25] Roman Yampolskiy: Threshers turn. Then you assess some decision by a system. You're doing it with respect to a specific time frame. Is this a good decision for the next five minutes? Maybe. It may be a horrible decision in 10 minutes, become wonderful again in 20 minutes, and kill everyone five years later. At what point do you stop going deeper and looking at consequences of those decisions?

[00:08:48] Roman Yampolskiy: That's not obvious. And this is just like a type of the top of the iceberg for all the things we already know might get us. So I am not fully optimistic about our ability to do this perfectly well on the first try.

[00:09:06] Allison Duettmann: What's the alternative then? I don't think that many people would really say that we're like in a position to do this perfectly, especially not on a first try, but I could like more emergent, gradually improving the offense defense dynamics and in specific ways, or gradually leveraging more powerful AI systems to help us align more powerful AI systems.

[00:09:25] Allison Duettmann: What's the alternative to the kind of perfect, perfectly predictable alignment from the start, the now we're safe scenario.

[00:09:33] Roman Yampolskiy: So it's not obvious that we have to create super intelligence, right? We're doing really well with narrow systems. We use the narrow system, for example, to solve protein folding problem, which was considered very difficult and possible for humans to solve directly.

[00:09:48] Roman Yampolskiy: We can do similar work in other domains, not just biology / healthcare, but pretty much anything can be done really well with a dedicated system. What is the requirement for creating something which completely dominates all of humanity and all domains at the same time. It's really just a game theoretic problem where no company can say, "Oh, we're going to stop at this point because competition will go on".

[00:10:12] Roman Yampolskiy: You have this race to the bottom, but really we can get all the financial benefit, all the trillions of dollars of free labor, cognitive, physical labor from systems, very similar to what we have today.

[00:10:24] Allison Duettmann: Interesting. Sounds a lot like also comprehensive ASA services from Drexler and, a few other bits that we've talked about in Gaming the Future, a book that we wrote on this topic.

[00:10:33] Allison Duettmann: And I know that Beatrice will dive a little bit deeper into this more optimistic version of like, how could this future world look like? But I'm really also curious to learn a little bit more about your background to provide some kind of coloring for the worlds that we'll dive in later.

[00:10:46] Allison Duettmann: And, Can you just say like how in your perception, as like having been around in the kind of like security, but also like emergent AI safety field for so long, how has that field changed, let's say over the last, 10 years or something, how have you seen gradually like people getting on board and how have you seen narratives changing in useful, perhaps not so useful ways, what's the kind of genealogy of some of the beliefs that we currently are dealing with?

[00:11:08] Roman Yampolskiy: That's a great question. So when I started probably about 12 years ago, it was really science fiction. There was no field and nobody took it seriously. We started doing pretty solid foundational work. Our assumption was nobody would be stupid enough to just, connect internet to it, open source it.

[00:11:25] Roman Yampolskiy: So a lot of early work was on how do you box it properly? What are the virtual environments? What is..., and you can see my paper on this topic, getting citations increasing. And then. three years ago, it just drops because they just...released it. They followed none of the recommendations, right? They immediately give access to all the users. They connected it to the internet and now open source is becoming a standard in it. So the things we.

[00:11:55] Allison Duettmann: Just so people know what you mean, for example, by boxing or air gapping, just in case people don't quite know.

[00:12:01] Roman Yampolskiy: So the idea was this could be a dangerous piece of software, like a computer virus. Let's study it in an environment, which is separated from the internet, has no access to do social engineering attacks on humans. Basically, something we can control inputs and outputs for, something we fully control how it learns what it can do. And we looked at different protocols, amount of communication, amount of information going in and out.

[00:12:29] Roman Yampolskiy: Basically, we could have studied it in a very dedicated environment, but it's useless. No one followed that path, right? So this line of research, even if it was more promising, which was shown anyways, it's going to be hacked, but we never even tried.

[00:12:46] Allison Duettmann: I guess one argument here would be the fact that, we're trying to develop it relatively open at the beginning also means that, we have more eyes on the ball.

[00:12:53] Allison Duettmann: We can have, more people playing with it, discovering possible flaws that, would otherwise be discovered way too late once it's super powerful. So I guess that's this kind of security trade off of, investigating something in this agate box in this bias rate capacity versus, actually playing around with it and trying to red team it that way.

[00:13:09] Allison Duettmann: Do you have any more thoughts on this?

[00:13:11] Roman Yampolskiy: All right. So that's the idea. And it works beautifully with standard open source software. Then you have a tool. Lots of people look at the tool, they discover bugs and it is wonderful. If you have an agent with access to 8 billion people for social engineering attacks, that would backfire.

[00:13:27] Roman Yampolskiy: And again, you have all the craziest malevolent actors who can now modify the Perfectly friendly system to be less friendly. It seems like it may not be a great idea to open source something that powerful. It may work for narrow AI systems, for tools, but I think for AGI and super intelligence, that's just insane.

[00:13:48] Allison Duettmann: I guess we are still at the point where we have more narrow AIs, right? And so the idea would be that, it's better to detect flaws in the existing systems before we build up to AGI or, build up in, in a way that we have specific flaws in there that have, could have been discovered by a wider community.

[00:14:04] Roman Yampolskiy: But yes, but we don't really fix the problems, right? The way we're working at right now, we filter them out. If a system is discovered to be horrible, evil, and racist and whatnot, we just put some lipstick on it and now it stops saying the inappropriate word, but it internally is still the same system.

[00:14:22] Allison Duettmann: I think that's definitely a pretty big current topic of debate.

[00:14:26] Allison Duettmann: We've discussed it quite a lot also internally with so many , I think, interesting like trade-offs on both sides. Do you have any other kinds of cruxes that have emerged in the kind of safety community over the years that you've been like a member of it?

Governance and Regulation in AI

[00:14:40] Roman Yampolskiy: There is a huge growth in governance.

[00:14:44] Roman Yampolskiy: People who said, okay, but technical solutions are not enough. We need political solutions. And that's growing heavily. There is, as the European AI act that is a lot of effort at a UN level. So definitely a lot of people and a lot of resources pouring into that. I'm not so certain given previous technologies which were regulated, it's likely to work.

[00:15:08] Roman Yampolskiy: If you look at things like spam, computer viruses, all that is illegal, right? As regulated as it can be, but it makes absolutely no difference. in my daily experience with my mailbox.

[00:15:22] Allison Duettmann: So what has helped with spam and so forth? And what could we learn from it for making AI systems safer?

[00:15:28] Roman Yampolskiy: So some technical solutions made it slightly more tolerable, but at the end, nothing really presented a full solution.

[00:15:36] Roman Yampolskiy: We still have ransomware. We have viruses. We have spam. And I argued in one of the papers that there is a fundamental difference between cyber security and super intelligent safety. Cyber security, you always get another chance. You can reset passwords, provide new credit card numbers. Whatever happened is just an annoyance.

[00:15:56] Roman Yampolskiy: With superintelligence, there is possibility of existential risk on the first bug.

[00:16:02] Allison Duettmann: So I guess the main argument would be, let's keep it narrow. Let's keep it such that we can have often Stephen's dynamics. Let's keep it such that we can like gradually make new versions more safe over time and we can patch things, have technical solutions to bids, but we just need to avoid it going like full on super.

[00:16:20] Roman Yampolskiy: At least for a while. We only had this very powerful systems for two years, but it feels like we are so behind. We need to build super intelligence quicker. We need more powerful processors. We're like, it used to people people said we're 20 years, 30 years away from AGI. Now I think prediction markets at five years. tops of big labs, two to three years.

[00:16:44] Roman Yampolskiy: And that's too long. We need to do it next year. We need to do it in four months. So that seems like miscalculating the difficulty of getting it right.

[00:16:54] Allison Duettmann: Yeah, I think timelines definitely on Metaculus I think dropped by 10 years in the course of a year or something, once progress started happening.

[00:17:02] Allison Duettmann: Okay, cool. Perhaps not so cool.

The Future of AI: Risks and Hopes

[00:17:03] Allison Duettmann: So what do you think does, what is the day in the life of someone, like you're working really in this field, you definitely spend some time in deep research. You spend some time working on some of the papers and like books and so forth that I like just trying to onboard more of a general audience into the field, right?

[00:17:18] Allison Duettmann: And then you're spending some time teaching, I would assume, how has that kind of like level of someone like approaching the kind of AI safety problem from this like longstanding security interest, how has your life changed? And is there anything that we should be doing more of anything that you think are, we're like a little bit misguided in the current way that we set priorities and in the researcher's time really like working on these issues.

[00:17:40] Roman Yampolskiy: So there is definitely a lot more action in this field, right? If I used to get invited to speak somewhere once a month, now it's three times a day.

[00:17:49] Roman Yampolskiy: So there is definitely a lot more interest, a lot more demand, but so much of that is what I call safety theater. People starting organizations, companies, they are doing something which cannot possibly work, but it feels good. It feels like you're busy doing something. You are out there and it's good. And it's good that there is at least awareness of it, but I don't think it's getting us closer to a solution.

[00:18:14] Roman Yampolskiy: I was just at the conference on specifically beneficial AGI. And the first thing the keynote speaker said was, "of course, we're not going to control superintelligence, it's laughable, of course not". And everyone agreed. And this is confusing because the kind of state of the art thinking was, of course we can do it, we just need a little more time, more resources.

[00:18:36] Roman Yampolskiy: But very quickly, I think it switched to where when I survey people on social media at conferences, majority doesn't think it's possible to control super intelligent machines, but it changes nothing about their day to day activities. They still work for the same labs. They still publish papers on some kind of mundane aspects of technological unemployment next year.

[00:19:01] Roman Yampolskiy: So I'm not sure what else I can really say in my talks. Usually I would Present my arguments, explain why the following are not possible, different tools you need for control. So we're likely to end up with very problematic outcomes, whatever it's existential, suffering risks. And after I conclude, I got any questions and it's always the same.

[00:19:25] Roman Yampolskiy: Will I lose my job next year? How do I properly operate sex robots? Like all sorts of things which have nothing to do with the main point or what I'm trying to convey. So I still haven't solved that problem of actually getting people to not just understand the conclusion here, but actually fully embrace it.

[00:19:45] Allison Duettmann: I guess to some extent you're making like two points. One is, some people are more worried about the near term implications, but then, just earlier you mentioned that others are also like really trying to speed it up even more, almost not having like willing to wait for superintelligence or AGI to arrive.

[00:20:02] Allison Duettmann: So how do you square both of these sides? Perhaps like they're made by different parties, but yeah. So maybe first that question.

[00:20:08] Roman Yampolskiy: So there are different camps, obviously there are people who think there is no problem to begin with. I have multiple papers surveying skeptical arguments for why There is nothing to worry about.

[00:20:19] Roman Yampolskiy: Something so smart will always be nice, for example, is a great one. We have no counterexamples to that, so clearly superintelligence would be delightful. They are not worried about negatives, so they do want to get benefits as quickly as possible, as much as possible. They want to be the ones to get there first.

[00:20:36] Roman Yampolskiy: Within the safety community, there are people who understand that it could be dangerous, but they truly believe that just given a little more time and a lot more money, they can handle it. Okay. That's more reasonable. And so there are degrees of how much you think the problem is solvable and how long it will take.

[00:20:55] Allison Duettmann: Probably also quite different communities. So if you think that, the main problem is just like, kind of like at least perceived race dynamics towards artificial general intelligence and like almost artificially speeding those up, then what could one do in your perception to keep AI narrow if it is more about kind of these game theoretic, yeah, almost artificially constructed or artificially accelerated race dynamics by thinking that you will have a first mover advantage, what might be actually in hindsight, accelerating the race.

[00:21:31] Roman Yampolskiy: So it seems that at least the top people at most leading labs I know are well aware of the problem of AI safety and have previously spoken about it, written blog posts showing they are very concerned. So my hope was that personal self interest, those are usually younger people, very financially secure.

[00:21:52] Roman Yampolskiy: It's not in their best interest to destroy the world. They will not benefit from it. It's literally the worst outcome for them. So if I can convince them that truly they will not succeed at this, I think it's there it's in their best interest to stop this. Unilaterally, even if it means someone else gets there first, it doesn't matter who creates uncontrolled superintelligence.

[00:22:16] Roman Yampolskiy: If it's uncontrolled, the outcome is the same. We're often told if we slow down, China will get there first. It makes no difference if it's not controlled by them. It's not important who messed it up. And you don't even get the usual benefit of being like the big bad guy in history. There is no history books.

[00:22:35] Roman Yampolskiy: You're not going to be remembered. So it's a pure loss. And if I can convince people that I'm right about that, maybe it will help. So I'm trying to publish additional results showing, okay, not only is it impossible to do X, Y, Z, but also monitoring new training runs. Does not allow us to predict capabilities of a system until much later with additional testing.

[00:23:00] Roman Yampolskiy: Testing is problematic because we don't know how to debug something like that. We know how to debug narrow systems with edge cases and specific domain of operation. How do you debug something general? Something capable of really operating across domains and doing it at a level you don't fully understand.

[00:23:19] Roman Yampolskiy: This is what I'm trying to do. Others are going, okay, let's convince the government to ban CPUs, ban graphics cards, unlikely to work in practice, but it's something.

[00:23:33] Allison Duettmann: So you're trying to really pinpoint why specific ways in which people think that you could make systems safe, you cannot actually make them safer, not reliably.

[00:23:43] Allison Duettmann: I guess there was also this really interesting report that recently came out from ARIA from Davidad and a few others where they're trying to move people from the perceived prisoner's dilemma into a perceived Stag hunt game theoretic dilemma, basically just like incinerating that if we could get a really good safety strategy in place that more people could at least believe in, whether or not that's now for AGI or superintelligence, but let's just make existing systems safer, then if we could get that kind of be credibly like a good collaborative effort, then people will be moving more likely to this effort.

[00:24:14] Allison Duettmann: And you'd only like me to move people from this perceived prisoner's dilemma, where everyone really is racing towards like an opportunity where they stand more to gain by cooperating with others on a possibly, like safer version where you could at least move people out of this kind of like race dynamic into more of a collaborative spirit.

[00:24:30] Allison Duettmann: So I guess part of what I'm saying is just like in a general sense, getting people perhaps also aligned around specific solutions where you could have the benefits of AI without racing towards the brink or without, really risking everything would make those outcomes more likely.

[00:24:46] Allison Duettmann: Do you have anything to say on kind of like these dynamics or like shifting the kind of current perceived race dynamics to more collaborative efforts rather than just by pointing out how the race will fail?

Challenges of AI Safety Projects

[00:24:55] Roman Yampolskiy: So there are different similar approaches. The idea being let's all kind of cooperate on one big safe project and defund all the bad, unsafe projects. But I'm concerned that you are really just pulling resources together, pulling compute, pulling all the best scientists. So that one project, so that will just accelerate capabilities to research. They still will not succeed at safety because I'm arguing you can't, but now they have all this extra resources to improve capability.

[00:25:29] Roman Yampolskiy: And if you remember, all the top labs, OpenAI, Anthropic, they were all product of effective altruism, trying to create safer labs to compete with unsafe labs of Google, Microsoft, and they are the ones who created the most capabilities progress very quickly. So I think it's very hard to separate pure safety work from capabilities work.

[00:25:56] Roman Yampolskiy: And the argument is we'll make a system smarter, so it will help us do more safety. But it never pays off that way. It's always now we have a much more capable system and the safety is still flat.

[00:26:09] Allison Duettmann: I don't know if their specific argument is let's get more intelligence to solve safety faster. And, they do have a relatively elaborate plan really on the security aspect as well, but I think more in general, I was just trying to make the point of, are there specific collaborative efforts that you would also want to point people to rather than perhaps like just pointing out the risks of racing towards the brink of what we could be doing this instead to incentivize collaboration into a specific direction?

[00:26:31] Allison Duettmann: Are there specific things where you like more research into this? That would be really useful.

[00:26:37] Roman Yampolskiy: That's a great question. I'm not aware of a specific project where I would say they progressing on safety while not making progress on capability. I cannot think of an example like that.

[00:26:49] Allison Duettmann: But are there perhaps specific things in the computer security realm, or, even in the cryptography realm or on any of the other domains, that you're like, are an expert in where you're like, at least we should be solving these problems as we go along.

[00:27:02] Roman Yampolskiy: In computer science in general, it's pretty standard to first decide if a problem is solvable. If it's impossible to solve, like a halting problem, you're not going to ask for people to start new labs and get more funding to solve it. Perpetual motion is another example. It's not the question of smarter people with more funding.

[00:27:21] Roman Yampolskiy: If you truly can show that the problem cannot be solved, you need alternatives, complete alternatives. Do not build this nuclear bomb if you cannot control the reaction. If I'm wrong and somebody can prove, no, actually, here's a bug in your code, your book is wrong, we can control it, then wonderful, then we can put more resources and maybe succeed at that, but that's not the case.

[00:27:46] Roman Yampolskiy: Again, just informal surveys, majority opinion right now, we will not control it. If you think about it again, you can probably solve it for an instance in time, a specific model, the specific time can be shown to act as designed, but to argue that you can do it indefinitely would violate the whole history of cybersecurity, computer science.

[00:28:11] Roman Yampolskiy: We never succeeded at building bug free software, even for mission critical systems where we verify code. It's still later discovered, okay, the verifier had a bug in it, or, maybe there is a side channel attack, which completely bypasses your beautiful crypto algorithm. So we just don't have a history of working at that level of guarantees.

[00:28:37] Roman Yampolskiy: Even if you get something, I don't know, one in a million chance where it's going to fail for a system, which is so widely deployed and makes so many decisions. At any given time, it's just, 10 minutes later, you're statistically guaranteed to have a failure.

[00:28:53] Allison Duettmann: I guess the question is also, is this failure, how catastrophic is the failure?

[00:28:56] Allison Duettmann: Is the catastrophic, is the, is if there is a failure, is it smaller than that, that you can patch it? Do you have enough folks who can like, or like enough intelligence really to bring to the challenge at that point to come up with a good solution and with a patch, or, one failure actually going to destroy the entire system that it's built on. And I think that, that is like a question that is still out. Would you want to say anything to that? I don't know.

[00:29:18] Roman Yampolskiy: Yeah, we don't know for sure and obviously statistically you are more likely to have a lot of small bugs than one major bug.

[00:29:25] Roman Yampolskiy: But if you look at the trend of AI accidents, and I have a paper where I just record historical accidents, the pattern is the system designed to x will fail to X, and then it's a narrow system designed for something simple. Your spell checker will misspell a word. Then you have a system for making scientific breakthroughs across all domains.

[00:29:44] Roman Yampolskiy: This could be problematic if you're talking about synthetic biology, if you're talking about nanotech, if you're talking about nuclear, one bug could be very significant.

The Complexity of Multi-Agent Systems

[00:29:56] Allison Duettmann: Yeah, I guess here the argument perhaps, and I think maybe it's an argument similar to the one that you're making, it's what if we don't just had one kind of like more the traditional singleton what if you didn't have just one agent, where one Paymo could absolutely be catastrophic, like the, traditional singleton, but what if instead you had like a collaborative ecosystem of a bunch of different agents cooperating with each other, each specialized on a specific sub problem that they are trying to solve embedded in this larger kind of, relatively computer secure, or like maybe even pretty boxed or like capabilities based system where, you one mistake doesn't escalate the entire system, but where it can be relatively quickly contained and patched.

[00:30:35] Allison Duettmann: So what do you think about those types of different scenarios? And could we be moving more towards the latter one? If you think it's more likely to lead to a secure, at least a more secure world.

[00:30:45] Roman Yampolskiy: So usually making a system more complex, a multi-agent system is harder to debug. It's harder to predict what will happen with it, predict future states of that system. If you have one agent and it's a narrow agent, you may be understanding what it's working on and what domain, and you can do some debugging, some testing. If you now have a society of those agents with different capabilities, interacting, communicating, you're really creating this super organism.

[00:31:11] Roman Yampolskiy: You have to zoom out and see. the system as a whole. And really what you did, you created this end colony. Maybe each individual end is not so capable, but the colony as a whole is quite dangerous.

[00:31:23] Allison Duettmann: And so then your alternative is maybe we just have one narrow agent that is then pretty versatile. So you could use it for scientific discoveries.

[00:31:31] Allison Duettmann: You could use it for, I don't know, just, other capabilities too. What's the alternative here?

Exploring Narrow AI Solutions

[00:31:34] Roman Yampolskiy: So I think, yeah, a specific problem is a great target. And again, the protein folding example is just beautiful, right? It's a very difficult problem. Helps us cure diseases, helps with life extension, but you have a very narrow system.

[00:31:47] Roman Yampolskiy: It doesn't know how to play chess, doesn't know how to drive cars. It knows how to fold proteins. It's super intelligent in that narrow domain. We can do the same thing in many other domains. We have many examples where we created super intelligent, narrow AIs. One domain, not general intelligence, cannot self improve, cannot engage in other activities.

[00:32:09] Allison Duettmann: Oh, then it is quite close to the world that I was at least trying to paint here of, the system in which you have very many different agents. How did you think that the two were different?

[00:32:17] Roman Yampolskiy: Allison, you made it sound like they are part of the same kind of boxed environment where they get to communicate and interact and do each other favors.

[00:32:24] Roman Yampolskiy: You solve this for me. I'll give you that. Whereas I'm talking about just a standalone agent with no other assistive super intelligences.

[00:32:32] Allison Duettmann: Interesting. Okay. So I guess then the difference was that in your world, the different AI agents wouldn't be able to talk to each other at all. And I guess in the larger economy or ecology or ecosystem that I painted, you possibly also have different, very specialized, super intelligent, but narrow AI systems collaborating with each other in secure ways.

[00:32:50] Allison Duettmann: And you think -

[00:32:51] Roman Yampolskiy: Right. They're not trained together. They're not grown together. They're not a single unit made up of modules. They're just standalone modules. We shall not in any way, relying on help from others.

[00:33:02] Allison Duettmann: Would they be allowed to talk to each other?

[00:33:07] Roman Yampolskiy: Ideally, you probably wouldn't want them to for safety reasons, or at least not directly.

[00:33:14] Roman Yampolskiy: If they can communicate, you basically making one system with multiple modules comprising it.

[00:33:23] Allison Duettmann: Yeah, here we are again at some very philosophical, or I guess, I was onto logical questions, but there's really interesting work coming from the cooperative AI foundation, basically on, like really trying to avoid deception and, multi agent settings and so forth.

[00:33:35] Allison Duettmann: And I think we're just like, have a lot to figure out in that regard. Okay, cool. I'm almost at the end of my time here. Thanks a lot for indulging me and all of you. I guess just different thought experiments here. I want to hand it over to Beatrice now to dive into some of the more positive worlds as we're wrapping up, like some of the exploration, at least of, a few of the bits that they've been thinking about.

[00:33:53] Roman Yampolskiy: Thank you so much .Sorry I didn't provide more solutions and mostly problems.

[00:33:58] Beatrice Erkers: Hopefully we can come up with some solutions or at least maybe not solutions, but just what it would look like if it goes well, if it goes, if we have positive progress.

[00:34:07] Beatrice Erkers: But I wanted to start because you mentioned your new book in the beginning and I wanted to maybe just hear you say a few words on: why did you write this new book? What are the key points that you really wanted to get across in this new book?

[00:34:22] Roman Yampolskiy: So I see a control problem as something we need to formalize. And in the book, I talk about different levels of control. You have direct control where you just give orders. This is like the genie problem, right? You give a specific order, it's misinterpreted, you regret it.

[00:34:38] Roman Yampolskiy: You have delegated control where you go, okay, you're smarter than me. You figure out what needs to happen here. And you obviously are not in control at that point. You are a child and somebody is babysitting you. So there are different problems. There's four levels and we can see how they are subtypes of those two extremes.

[00:34:56] Roman Yampolskiy: But whatever specific control problem you want to concentrate on, you can realize you need certain tools, a toolbox of capabilities to make it right. You need to be able to understand how the system works. So explaining internals. Explaining neural network weights and what they represent and why they activate it.

[00:35:18] Roman Yampolskiy: You need to be able to predict what decisions the system is making, not just as a final step, but as an intermediate step. So if I'm playing a chess system, I know it's trying to win the game, but do I know what specific moves it's going to make? If it's smarter than me, I don't, I cannot predict it. If I could, I would be smarter or equally smart.

[00:35:39] Roman Yampolskiy: So we don't have predictability. We don't have explainability. We have a survey paper with about 50 different tools, which we would love to have to make this easy to solve, but we don't, or at least we don't have it to the degree we would like to have it. And so if you look at it as a whole control becomes likely impossible.

[00:36:00] Roman Yampolskiy: And if I just say it, okay, I think it's impossible. Nobody's going to buy it. So I go on a survey in all different fields in psychology and mathematics and obviously computer science, but every field I could find relevant to this, what are the different limits, known impossibility results? So we know.

[00:36:19] Roman Yampolskiy: In public choice, there are limits to voting. We know that certain voters will get screwed no matter what voting system is being utilized. There are limits in physics, there are limits in economics. And if you look at all of them, they are relevant, they are significant. Maybe I can do well without a specific tool, use something else instead.

[00:36:40] Roman Yampolskiy: But I think there is more limits than actual capabilities. And if you start looking at the field of AI safety, almost every paper is something like we looked at this problem, we have a toy solution, which doesn't scale to the big picture, but we discovered 10 new problems. Which we're going to work on later.

[00:37:00] Roman Yampolskiy: It's like this fractal nature of a problem. The more you zoom in, the more you discover additional problems you didn't know about. If you look at old papers, we were worried about specific things. And now we discovered that there are 20 other sub problems within that. And most of the time we keep. discovering new problems, but very few papers go, and this is the final word in this space, and we solved it and no one has to worry about it.

[00:37:28] Roman Yampolskiy: This is the final solution to the inner alignment problem.

[00:37:32] Beatrice Erkers: And what do you think of something like an approach to differential technology development or something like that's been discussed more recently? Is that something that you would get excited about?

[00:37:41] Roman Yampolskiy: It would be wonderful. It's very hard to separate safety work from capabilities work.

[00:37:47] Roman Yampolskiy: In fact, outside of purely theoretical work, I think it's impossible. And there is very few people who do purely theoretically AI safety work. So Yudkowsky is a great example. I don't think I ever contributed to general capability. I made contributions to narrow systems, but never the general, everyone else works mostly on capabilities.

[00:38:07] Roman Yampolskiy: They are famous for their capabilities work. If you look at top safety people today, they got their Turing awards, they got their recognition for making very capable AI systems.

Future Visions and Governance

[00:38:18] Beatrice Erkers: So I guess I'm going to try to start us towards seeing if there are any sort of outcomes that you think could be hopeful. I'm interested in, you discussed, narrow AI systems can be very useful. You've mentioned that a few times. I think that's a very interesting constraint. For example, we're doing a world building challenge at Foresight currently, where we, that's a constraint that we give people when they ask them to build out the world in 2045, but we don't have AGI, but it's a very hopeful vision of the future. So what does that world look like? What did narrow AI help us achieve? And I'll leave it to you if that's how you want to frame your vision of the future, because I'd like to know if you think of an existential hope scenario for the future, and I'm thinking, especially in relation to, since you're so specialized AI, it would be very interesting to hear if you think, if it went well, what would that look like?

[00:39:08] Roman Yampolskiy: So maybe we can look at specific problems we're interested in solving and then creating a targeted AI, which looks just at that problem. I think aging is a disease. We can probably cure it with a very simple modification to DNA where, okay, you have this loop. It's set for 120 iterations. I change it to be an infinite loop minus cancer.

[00:39:31] Roman Yampolskiy: And now you live forever. That's wonderful. I don't need to do anything else. Like this is a specific good outcome for everyone. And I think we can get there without super intelligence.

[00:39:43] Beatrice Erkers: Are there any other technologies that you'd be excited about that does not have to be AI, but that, maybe could be enabled by AI that you just think the world would be better off if we had?

[00:39:55] Roman Yampolskiy: Again, we have so many advisor jobs for different humans. You have your financial advisor, you have your You know, relationship coach, you have all those things could be very narrow AI systems telling people who may not be experts in a domain or maybe intellectually not at the top of their game. Okay, this is better if you invest money in [ ] versus VC[ ] again, no super intelligence required, just automating a very specific set of skills, which I think should have been automated a long time ago.

[00:40:27] Beatrice Erkers: Yeah. I think you also mentioned, there's a lot more governance people getting involved lately in these questions as well. Are there any sort of governance mechanisms or anything like that, that you're excited about in relation to AI safety?

[00:40:39] Roman Yampolskiy: The government itself can definitely be improved with technology, both in terms of more direct representation. And in terms of efficiency of how the system operates, I don't think anyone would argue that many of our politicians are super intelligent. So it should be quite easy to replace some of their functioning with narrow systems.

[00:41:03] Beatrice Erkers: That's, yeah, that's interesting. Is there any specific like event or breakthrough that if it happened in the next few years that you would think, Oh, actually we're on track to maybe making things work, like anything that would make you think that we're actually on track to a positive future scenario rather than all the doomy ones that are possible.

[00:41:27] Roman Yampolskiy: As I said, this is all about the timeframe you look at. So a specific discovery can make me happy because I think, oh, we just bought five years of extra time. This is wonderful. But long term, the super intelligence you create will itself create another super intelligence. This will do the same. This is an infinite process.

[00:41:45] Roman Yampolskiy: It will never stop. There is never a point where we go, we just solve the AI safety. We can all go home now. This is a permanent solution. We don't have to worry about it. It's an infinite problem. The space of possibilities keeps growing exponentially. So I don't think we'll ever get to the point where we all go home.

[00:42:06] Roman Yampolskiy: Sorry.

[00:42:08] Beatrice Erkers: No, that's okay. We don't- I think most people would agree with you on that point. If you would, this is a difficult question, I think maybe, but If you do imagine yourself, it's 2045, things are looking pretty good. What does Roman do on a day, a good day in 2045 when things have gone well with AI?

[00:42:26] Beatrice Erkers: What's a day in the life of a positive future in that scenario?

[00:42:30] Roman Yampolskiy: Pretty much like today, but papers are not about safety. I have freedom to look at other topics. How to break the simulation.

[00:42:39] Beatrice Erkers: And today, like you're just like, you're free to dive, deep dive into anything that you're curious about, or just, yeah, spend your time.

[00:42:46] Roman Yampolskiy: not about just self protection and trying not to destroy the world, but we are free to explore beyond these immediate concerns, kind of like the muscle of the pyramid of philosophy. We got the base substrate secured. Now we can look at what's out there.

[00:43:02] Beatrice Erkers: Yeah, like being able to focus on your own self realization rather than survival and these sort of things.

[00:43:07] Beatrice Erkers: Yeah, I think that's something that most people would be really excited about. Some people are already experiencing it today, but maybe not aware of most of the risks happening. For if you want to onboard someone and get them excited about working on these challenges that we've discussed today, what would you recommend?

[00:43:24] Beatrice Erkers: Any special resources would you recommend, other than your book, obviously that's recommended, but anything else to get onboarded to these, the work that you're doing.

[00:43:33] Roman Yampolskiy: There is no shortage of resources. If anything, the problem right now is it's almost impossible to be fully caught up to the state of the art in the field.

[00:43:41] Roman Yampolskiy: Then I started, I literally read every safety paper ever published and surveyed them. Then I would read only the good papers, then only the best. And now I don't even read titles of the best papers. I don't have time. And that includes summaries by GPT 4. So at this point, I'm like every day becoming less and less expert in my own field.

[00:44:02] Roman Yampolskiy: Yeah, if you can solve it for me, I would appreciate that.

[00:44:06] Beatrice Erkers: Yeah, I will try maybe better for an AI than me. Yeah. Is there anyone else that you think is like an inspiring actor in this field? Like anyone you think we should have on this podcast, perhaps?

[00:44:17] Roman Yampolskiy: Have you had Eliezer already?

[00:44:20] Beatrice Erkers: We have not had Eliezer. That would be very interesting to have him. Yeah.

[00:44:24] Roman Yampolskiy: He's usually a couple of decades ahead of his time, so I would suggest that.

[00:44:28] Beatrice Erkers: Yeah. Yeah. Definitely worth a try. I don't think we've even tried yet. I think I was a bit afraid of what he would come up with in terms of, it would be very interesting to hear his existential hope scenario if he can think of one, but.

[00:44:40] Roman Yampolskiy: I'm worried it involves Harry Potter somehow.

[00:44:43] Beatrice Erkers: For you, but is there anything that you think we have missed discussing that you would like to make sure we get to? No.

[00:44:50] Roman Yampolskiy: No, I think you covered all the interesting aspects of this field.

[00:44:54] Beatrice Erkers: Great. The last one is slightly just a bit of a surprise question.

[00:44:58] Beatrice Erkers: Oftentimes people get a bit surprised and thrown by it, but it tends to be interesting the responses we get. The question is, what's the best advice you ever got?

[00:45:07] Roman Yampolskiy: If you care about the opinions of other people, the best you can become is average.

[00:45:14] Beatrice Erkers: I think that's very good advice. And that was a very interesting answer.

[00:45:17] Beatrice Erkers: So I'm happy I asked. Great. Thank you so much, Roman, for coming on the podcast. Really appreciate all the work that you're doing and am very happy to be able to share your work with the audience of this podcast. So thank you so much.

[00:45:30] Roman Yampolskiy: Thank you so much for inviting me.