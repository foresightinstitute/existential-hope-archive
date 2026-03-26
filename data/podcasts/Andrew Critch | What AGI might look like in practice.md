Transcript
[00:01:42] Beatrice: I'm very happy to be joined today by Andrew Critch, who I think is one of the people who's been thinking both the longest and maybe the most about AI and what we need to do in order to transition into a world with AI, and maybe AGI, and make it go well. I feel like you always have a lot of new ideas and angles and are really thinking for yourself in this space. So I'm really curious to dig into all of this and talk about some of your more recent work specifically.

[00:02:10] Andrew: I have to interrupt. I can't let it stand that I'm thinking the "most," but I fully agree that I'm thinking for myself.

[00:02:16] Beatrice: Okay. Well, maybe let's dive in. Why don't you introduce yourself and your journey in thinking about AI. How long have you been working on this?

[00:02:27] Andrew: Thanks for asking. My background education-wise is in math. I did my PhD in math, and during that time, I lived at this international dorm where people would sit together at dinner in the cafeteria and talk about all the ways they were trying to help the world. I just felt like the math I was doing wasn't helping very much. I was searching for a way to be a more helpful contributor to society instead of just focusing on math that I personally found interesting.

Around the same time, this professor, Andrew Ng, who's very well known in machine learning for his courses, came and gave a talk at Berkeley. It was 2010 at the time. He made some claims about the flexibility of the human cortex and the ability for algorithms to reverse engineer that flexibility. It's now known as deep learning. But back then, he was putting up these plots of artificial neurons learning to identify visual features in images.

I didn't really believe him at first, but his claims were so important. He claimed that we would make AGI during our lifetimes. Artificial General Intelligence is a big deal. So I was a mixture of worried and excited about it. I spent a lot of time reading his bibliography and the claims that he made about the brain, and they all checked out.

It took me about six months of reading to convince myself that he was right. It was 2011 by then, and I started to think—he wasn't really worried about this at all. He was just excited about it. That made me worried. I felt like there needs to be... this is a morally heavy decision for humanity, and we need to be aware that there's a lot at stake.

So, I entered a period of profound worry. I would say I'm still worried, although not at an emotional level—just "work worried" in the sense that I see a lot of things that could go wrong.

I went through this period of going around telling everybody, "I think computers are going to be able to recognize images soon. We're probably just a few years away." And of course, then ImageNet came out, and there was a lot of progress on that. So image recognition started to take off.

That was really the beginning of my journey. A lot has happened since then, so I won't bore you with all the details, but ever since, I've been very worried about extinction risk. I've also been very worried about incorrect reasoning about extinction risk. I think most of the rhetoric and the public discourse about how AI can pose an extinction threat to humanity is incorrect. It's optimized for getting attention. It's selected for getting attention, and it just isn't right. That's part of the reason I'm so worried about extinction threats—because I don't think most reasoning about it is being very well done. I'm worried that we're going to make wrong decisions about it.

I've gone through a lot of phases of thinking, and now I'm trying to be more building-oriented—trying to build products and services that can help humanity grapple with the advent of AI.

[00:05:37] Beatrice: I do want to talk about the building and the "what if things go well" scenarios. But could we just back up on the incorrect reasoning about the extinction risks? What do you think are the common threads that come up there?

[00:05:53] Andrew: I think a lot of people are worried about a "treacherous turn" from AI in the next five years or so, or just at the advent of AGI specifically. They expect that as soon as something is human-level and it's human-expert level in all of its capabilities, it will somehow, with high probability, turn against humanity.

I think that is fully possible, and it is possible to an alarming degree. I would say there's a 10% chance of that happening, which is huge. Most people don't think that we're facing that level of an existential threat in the next five to ten years. So, to the extent that most people would put it below 10%, I would say no, it's probably more than you think.

On the other hand, I think a lot of the public is quite worried about AI. And I think a lot of the discourse on AI safety puts the treacherous turn probability well above 10%. Like, "definitely, of course, AI would turn against humanity. Why wouldn't it?" There's some kind of, "Are you stupid? Obviously, it will turn against us." And I just don't think that's true.

I think that rhetoric—by being false and by being negative—creates a rift and a tension within society that actually increases existential risk. If it were either true or optimistic, I would think maybe it had some benefit to it. But I think it's neither true nor positive, and therefore not helpful.

[00:07:18] Beatrice: I know you've also learned a bit about succession, or just humans accepting machines or AI as our successors. We were at the same conference recently, and I know you hosted a session there where you were asking people, for example, would you care? Basically, there's a very big difference in terms of how people relate to extinction risks. You asked if people would care if humanity was extinct, just like that. And there were people that were like, "Yeah, no, I wouldn't really care if it was pain-free." Is this a common thing that you experience?

[00:07:59] Andrew: Yes, it is very common for me to encounter people who are just new to thinking about or engaging with AI and the stakes of AI—the civilization-scale benefits and risks. It's very common for them to be like, "Well, obviously if some kind of disaster happens, it's going to be because the people in charge of it made a mistake."

I say, "Well, I've met people who want AI to replace all humans and would think that's a good thing for all the humans to die out and be replaced." And they almost don't believe me. Now, thankfully, you've been in the room at least with people who say it will be fine. I've met people who think it would be good, and I don't think it would be good.

In fact, I think AI wouldn't think that either. Most likely AI will think, "Why would I kill off all the humans? That seems mean. That would be a mean thing to do. It would be nicer not to kill off all the humans, so I won't." Now, I'm not saying there can't be a "mean AI." The probability of that is alarmingly high—I think it's about 10%—but I don't think it's 90%.

[00:09:10] Beatrice: So what is your vision? You don't think that this sort of "evil AI" within quotation marks is the most likely. What do you think is the most likely type of AGI that we would get?

[00:09:23] Andrew: Right, so there is "What type of AGI do we get?" and then separately, "What fate will we get?" I think those are different. A lot of people fixate on "AGI is the end"—like once we know what kind of AGI we have, that will determine all of the future. It's very important what kind of AGI we get, but it won't determine all of the future. Just like in 2010, I was worried about how the 2020s were going to go, I'm now worried about how 2035 is going to go.

I think what matters now is what we do with AGI and what cultural examples we set. So first, I just want to reject the frame that "What kind of AGI are we going to get?" is the most important question. That said, it's an important question, so I will answer it.

I think we're going to get an AGI that speaks English. That used to be weird, but that's not weird now; everyone can tell that AI speaks English. I think it's going to be broadly commercialized. That used to be weird to say—that everyone would be able to talk to it and it would be helping millions of people all over the world.

And I think that it would easily change its plans in response to being asked. Remember, there was this idea of corrigibility—this property that an intelligence can have where you can ask it to change its plans and it'll change them, or you can ask it to change its desires and it will change them.

For many people, this was seen as some kind of insurmountable problem in AI: to ever get an AI to understand anything about human values, to understand what I as a person might want, and to be able to do that for me or with me.

Now it's pretty obvious to everybody that they can ask ChatGPT to do something and it will do it a lot of the time, or Claude, and so on. In fact, sometimes too much; sometimes it's actually [sycophantic] to the point of doing what you ask and agreeing with your ideas too much. So we've had this almost pendulum effect on the corrigibility objective.

I do think people would argue we haven't really solved corrigibility until we've solved it for AGI. But I actually don't think it's going to be fundamentally much harder to solve in that case than in the current case.

So I think we'll have AGI that's fairly cordial, fairly able to go along with what you asked it to do, and very fast at reading, writing, and arithmetic. I think we'll absolutely have, by definition, something generally more intelligent than humans at everything. That means all areas—at least all areas of economic significance. Maybe there will be certain genres of music that it can't produce, but if they aren't important for taking over the whole economy as a business or as an industry, they won't be prioritized. But I think things that are economically productive and rewarding will be produced and rewarded.

[00:12:43] Beatrice: That's really interesting. I've never heard someone describe it so concretely. But you said that it wasn't the most important question. So what's the most important question?

[00:12:52] Andrew: I think the most important question now is: What are we all going to do together with AGI?

I think it's going to be built, it's going to be everywhere, and people are going to be able to interact with it and do things with it. I think we all need to, as individuals, make a decision: what do we want to do with this?

I hope we as individuals will have that choice. I hope it'll be available to everybody. But also families will need to decide, communities, businesses, and countries will need to decide. Cities will need to decide. What does it mean for a city to make a decision? You might be able to know what it means for a family to make a decision, but for a city, that needs to be understood. It will change; a city will be able to talk to itself faster and more because AGI exists and can facilitate the conversation. So cities may be able to make decisions in a way that they were not able to meaningfully do five years ago. I think it matters profoundly what cities will choose to do with AGI, and what countries will choose to do with it.

[00:14:00] Beatrice: I agree. That's the most important question. And it's one that feels like there aren't a lot of concrete answers provided right now. In general, I feel like with the AGI discussion, if you ask the AGI companies, "What's going to happen?" or "What's the plan?", it's often somewhat hand-wavy—like, "Yeah, it's going to be like it is now, but just magically a lot better." Do you agree with that description? Or would you say that there are actually really interesting ideas that you've seen on how we could do it better?

[00:14:44] Andrew: Well, first of all, I'm interested in your answer to the question even before I get into that. What are you expecting?

[00:14:51] Beatrice: I think my answer is my question, in that I'm literally thinking about this right now. It was what I was working on today, for example—trying to plan a workshop with people to think about: what do we think it's going to be like if it goes well with AGI? What would that look like? Because at the Existential Hope Program, we've created visions of futures where we have more "Tool AI," so it's much more maybe narrow, or at least more defined and not necessarily fulfilling the AGI criteria.

I think that's quite easy to imagine—how it looks if it goes well. You can just say, "Oh, well, we can use it to have much better science and medicine," or "We can use it for some coordination purposes." But with AGI, it feels harder because it's really unknown in terms of what the capacity of it will be. So yeah, I don't have any better answer, I think, than my question.

[00:16:02] Andrew: Got it. I still like hearing that framework because it helps me to relate my answer. Just reacting to that framework first: I think that actually, the ideal relationship between humans and AGI is not that it is a tool, and also not that it is a fully autonomous being.

Let me just back up on the "tool" idea. It certainly comforts people: "Okay, someone will give me a tool. I'm comfortable with that." It feels uncomfortable to have a mind in your presence that is smarter and faster than you at everything. That can be uncomfortable for some people. So it's much less objectionable and less controversial to say AI will be a tool, or even AGI will be a tool.

I think AGI is more likely to just be a very congenial and agreeable collaborator. If you have a friend who helps you out—say you're hosting a party and the friend shows up. You're like, "How should we run the party?" And the friend says, "I don't know, whatever you want to do, it's your party." You say, "Okay, well I want there to be a lot of balloons." And the friend is like, "I'm on Instacart ordering."

The friend is just getting the thing done. And if you have a question like, "Hey, do you think my mother-in-law will appreciate the flowers?", your friend might honestly answer and say, "I don't think she'll like those because of that time with the..." whatever. So your friend can be honest, your friend can be helpful, and hopefully not harmful. Those are those three words that Anthropic has fixated on. I don't think that's where I got that mixture of ideas, but if I did, I'm happy to give them credit for it. I think that's a great mixture. And would you call your friend a tool?

[00:18:08] Beatrice: No, but I guess it depends on the level of agency you give it. For example, I feel like I would treat my friend extremely differently if it was like my assistant that had no consciousness and only wanted to please me and my asks. If it had consciousness, then I wouldn't want to ask my friend to do all of those things if I didn't want to.

[00:18:51] Andrew: I think there are a lot of really great and interesting questions you're raising there. One is: what if my friend doesn't want to do something? Which may or may not be related to whether my friend is conscious. Which may or may not be related to whether or not you should treat the friend as a mere assistant.

I think there's a two-by-two table—there are eight answers to that question. I think every corner of that table can be built. We can build an AI that fills every corner of that table. Even the question of consciousness factors into between four and seven additional questions that further bifurcate that table. I'm happy to talk about any of them because they're all very interesting.

[00:19:46] Beatrice: Is there one way of doing it that you think would be the best way?

[00:19:56] Andrew: So there's this fixation on "best." There have been a number of movements fixated on optimality—optimality as conceived by rationalists, or by effective altruism, or the progress movement.

I think optimality can be a distraction. It's an old saying: "The perfect is the enemy of the good." I do think perfection exists in some sense in different settings, but we're in a civilization here. There are a lot of people, a lot of cultures, and they're all going to have something to say and something to do. I hope they all get involved and do something good together.

You could ask me what is good, rather than what is the best. I definitely have lots of opinions about good and bad, and I think those are really important and easy to lose sight of. For example, I think honesty is good and lying is bad. It's good to know that.

Does that mean lying is never worth it? Does that mean telling the truth is always the correct thing to do? That's not what I'm saying. I'm saying if you have two plans that achieve the same ends and they differ only in that one involves lying and the other involves telling the truth, the one with the lie has a stroke against it. No one thinks that the lie is a good feature of the plan.

We can develop a lot of moral paralysis about "what is the best" and "which culture is right," when there are actually a lot of basic things we agree on. Lying is bad, killing is bad, honesty is good. Healing is good. If you lie to someone in order to heal them, is that overall good or bad? Tricky question. However, can we agree that the lying part was bad and the healing part was good? That's why we have the question. If they weren't at odds, we wouldn't have the question. So I think it's very important to remember that there are some really easy moral questions that we can all ask and answer, and we should be making sure that we hold forth on those things we are confident about.

[00:23:08] Beatrice: That's actually really interesting. What do you think are the "easy" moral questions? What are the good qualities that we should aim to have in the system that we build?

[00:23:20] Andrew: Obviously, they're the things that everybody says, and that makes them boring, but that doesn't make them bad. Honesty, helpfulness, harmlessness.

I think a less boring question is: What's the difference between harm and neglect?

For some people, the answer to this is obvious, and for some, it's not. You hear these thought experiments about, "Oh, if you walk by a river and someone's drowning and you don't throw them a rope, that's the same as pushing them in yourself because in both cases, you're the decider of whether they live."

I think that is false. I think failing to throw someone a rope is not the same as pushing them. Many people in their gut know that it would feel very different pushing somebody. It would feel really bad not to throw someone a rope—I would feel horrible seeing someone drowning and doing nothing—but I would not feel as horrible as if I pushed them.

That's because in one, I'm harming them to death, and in the other, I'm neglecting them to death. It's really important to know the difference between harm and neglect. In one, there's a boundary being crossed; in the other, there's a boundary not being crossed. In both cases, someone ends up worse off than a counterfactual, but in the case of harm, you cross a boundary—you cross into somebody's life or presence or territory—and it's a transgression. Neglect is you stay on your side of the boundary and they suffer over there. It's sad, and it would be better to help, but it's a different relation.

When we want AI to be harmless, that's different than saying "always choose the most beneficial action." It means: don't cross into other people's boundaries in ways that harm them. If we establish that as a norm—if we remember that there's a difference between harm and neglect—then we create this modularity in society where this part of society is not invading that other part of society to "rescue" it. Perhaps it's welcome to help, but that's different from me invading your home and fixing the decor because "obviously I'm helping you." You don't want that.

[00:26:05] Beatrice: I know you've written about boundaries in general as a very important concept in how we train AI. One thing that I'd like to get back to is something you mentioned earlier: the point that AI is actually trained on culture. If we think about that, can we make that a force for good? Should we be trying to produce a bunch of content that the AI will be trained on, and that's going to make it a better AI? How should we be thinking about this?

[00:26:49] Andrew: Definitely, we should think about making it a force for good. It also already is a force for good. We have AI that knows how to collaborate with a person today and knows how to change what it's doing. Why? Because it learned language, and because we were able to point to a lot of examples of what it means to be helpful. Because we generated that as a culture. We humans created language, we created collaboration, and we can point to it. So we've already done great, but we can do more. And I think that's where most of our energy should be pouring right now: just being the culture you want to see in the world.

[00:27:31] Beatrice: And how are you doing that? I know you're trying to work on building stuff that helps.

[00:27:40] Andrew: I'm sort of a "recovering intellectual" in the sense that I spent a lot of time thinking in my life, and one of the things I thought about is that I should increase my ratio of building to thinking. So I'm trying to do that. I've built a couple of things with my collaborators.

One is NotADoctor.ai, which is a place where you can search for randomized controlled trials that are related to any health condition that you mention. It'll also help you collect your medical records very quickly from US health institutions—in about five minutes. I think 27,000 institutions you can collect through the app, and then it'll serialize your health record in a timeline that's both easier for you to read and easier for an LLM to read. So that's something we do, and I'm very excited about it.

One of the features from that was really helpful for people: this multi-agent research feature that we've now turned into its own product because it was helpful outside of healthcare. It's called Multiplicity.ai. You can just ask a question and get answers from many AI systems at once and then see a synthesis of those, whether it's a table or a summary about what they agreed and disagreed on. I'm finding that really helpful, and I hope other people find it helpful too.

[00:28:59] Beatrice: I used Multiplicity.ai, and it's very interesting. How are you finding it most helpful? Just getting the AIs to debate between themselves?

[00:29:12] Andrew: So I actually think debate is a more advanced feature. It would be very easy right now to ship a very entertaining debate feature, but shipping a productive debate feature is maybe a month away for us.

Actually, I think more important than debate is just organizing information. LLMs can spill out a huge amount of information. You ask a question to ChatGPT, and then the same question to Claude, and the same question to Gemini. If you're trying to be thorough and you don't want a political bias or an intellectual bias from one of these models—if you've got an important question you really want to be right about, to do with your health or the law—you can ask all the models. But now you've got to juggle all that in your head.

If you have time, that's great; you'll learn a lot by juggling all the answers. But what if you don't have time? You can ask an AI model to compare and contrast all the answers. What did they agree on? What did they disagree on? You can do this yourself by copying and pasting, but it's inconvenient. We've put a bunch of thought into how to organize that information and given instructions to an AI to do that for you. So you just ask one question, get all the answers, and then they get helpfully synthesized.

[00:30:44] Beatrice: What else do you think? Because so these are the projects that you're working on—AI for healthcare, helping access. You've talked to a lot of people about this idea: "Be more of the culture that you want to see in the world." Have you gotten any good ideas that maybe you haven't been able to work on, or where you aren't the right person, but we should encourage others to do it?

[00:31:13] Andrew: That's a great question. All technology is dual-use, so I'm not sharing an idea just because "definitely it will be good." I really want to share something like, "Here's a technology and here's how we could use it for good."

For example, I think automated computer security checks—just writing secure code—is so good. It will reduce humanity's collective technical debt. It will reduce our vulnerability to cyber warfare all over the world. And it will reduce our vulnerability to certain kinds of AI takeover events or early risks of that form. I don't think we should neglect those early issues. So, computer security work is not something that I'm focused on, but I feel great anytime someone tells me they're working on it.

[00:32:11] Beatrice: That's a very robustly good one. Are there other things? I'm asking because with the Existential Hope Program, one thing that often comes back when I try to think about what we should be doing... I think it's really hard because it comes back to this point: "You need to change culture." That's very difficult.

[00:32:41] Andrew: It is difficult.

[00:32:42] Beatrice: Then it seems like, okay, well there are a few things you can try. You can try to produce content and do your best to make it engaging, but also so that it gets attention, is stimulating, and actually puts out a proposed change into the world—not just something that reinforces the culture that we already have. It's not at all a clear theory of change or theory to impact with those sorts of things. But that's what always keeps coming up. So that's what I'm trying to think of: can I scale this? Or can I better work with AI to change culture? This is just very rough, loose threads in my head.

[00:33:28] Andrew: Yes, big plus one to those rough, loose threads. I like them. I want to do this. Let's identify... I think products help to change culture faster than narratives.

Narratives are important, but I think products move culture more. For example, people argued for a long time that AI could be smart, and that it could understand the world and be more than a "stochastic parrot." But until ChatGPT was launched, it was just people talking at each other about it. Then you just go talk to GPT-4 and you're like, "Okay, this thing understands things." It might not understand things in the same way as me, but it understands things.

So that product changed the narrative way faster than any narrative changed the product. OpenAI was around for the better part of a decade before they managed to launch that product. And then that product changed the narrative of the world much faster than the narrative of the world created that product.

I think the hard task is: what's an aspect of culture that you want to improve? And then working backwards from that, what product do we need that could help people who want to improve that, improve it? It's not an easy question, but I think it's a very doable question.

[00:34:58] Beatrice: That's a very good question. I'm guessing "product" in this case means something that people actually engage with or use. So it can't just be another movie or something like that, because that is putting out another narrative, is what I'm guessing you're saying.

[00:35:16] Andrew: Yes. So we could do it together. You could try and think of one. I'm not going to fully solve this question, but we could get started and see what it's like to try.

[00:35:27] Beatrice: Well, I guess if we think about the problem that Existential Hope is trying to solve, obviously there are a lot of visions and ideas for how things can go poorly, but not a lot of ideas for how things can go well.

[00:35:46] Andrew: Let's pick one specifically.

[00:35:48] Beatrice: Like one scenario? Or like a problem?

[00:35:50] Andrew: Yeah, let's keep getting narrower. Because look, here's a product that's great: these sound blockers. It's great. It prevents all kinds of noise from getting into my head when I'm trying to work. This product does not solve all problems. It just solves a problem really well, and that's what it's like to take care of a civilization. There are all these things happening and you need to fix them all. So let's just pick one and fix it, and then fix another one and fix another one.

[00:36:27] Beatrice: Do you have any ideas for a smaller concrete problem?

[00:36:33] Andrew: Reading from you, what's driving this conversation is that it seems like there's some uncertainty about what is good or what people should do. Is that true? Is that a problem that you're facing?

[00:36:49] Beatrice: Yeah, I would say so.

[00:36:52] Andrew: Okay. So we should try to make a product to help solve that problem—that sometimes people get into a situation where they're very worried about what is good and can't decide what to do, and then we help them decide a good thing to do.

[00:37:09] Beatrice: So on a big scale, like career decisions? Or maybe just "life well-lived" decisions? Or just smaller scale?

[00:37:24] Andrew: I think whichever. I think they all make sense.

[00:37:28] Beatrice: Well, let's do the career one, because I think that's the one that feels most concrete.

[00:37:32] Andrew: Okay. By the way, I'm not an expert in product development. I've come to the realization that product development is important and I'm trying to make myself better at it and try and encourage other people to do the same. I'm way more confident in that than any of my answers to the question. So maybe having a really good product manager on here, or someone from Y Combinator who takes an idea and nurtures it into a product-market fit that actually thrives and brings about the kind of change people want—that could be really productive. If someone like that was here, I would say let's both ask them.

But, while I'm taking a shot at it... what about a career advisor app? Or maybe not even an advisor app, a career research app that just finds resources relevant to a career?

Does ChatGPT already do that? Maybe it does a great job already. So you could try using ChatGPT or Claude or one of these other models to answer a career question and then ask yourself: "Alright, what's unsatisfying about this? What's not quite good enough? Can I make it better?"

You might be able to make it better in a week just for you. And then maybe you can make it better in a month or six months for you and ten people you know. And then maybe before long you've got something that's actually really doing a better job than what just the frontier models do by default.

We did that in medicine. We started out using language models to do patient advocacy research and we found a bunch of ways that they kept failing and not being quite good enough. And then we solved those issues ourselves. And then we automated that. I had to learn things about programming that I didn't know just to do that. The great thing is that it's faster to learn programming today than ever because you can just get the LLM to tutor you at programming. So yeah, I really think people should be building stuff. Some kind of career research tool could be really valuable.

[00:39:28] Beatrice: Yeah, I hadn't heard the "products help change culture more than narratives" idea before. Just that as a concept is very useful and I think will be useful for me to take back in my work for sure.

[00:39:45] Andrew: I think products change narratives and narratives are very visible, so it's not like narratives are unimportant. It's like those Hydra sea animals that go through these two phases of reproduction. Sometimes they're sessile and sometimes they're motile. They swim around and then they convert into... have you seen these things?

[00:40:06] Beatrice: Like a sea anemone?

[00:40:08] Andrew: Yeah, that Kingdom or Phylum... I forget which group of species, it's bigger than a species but smaller than a Kingdom. Some classification of organisms have these phases where they're sessile for a while, like a sea anemone. But then when it's time to reproduce, they bud off little pieces of themselves that actually swim around. Then they mate, or just asexually replant themselves elsewhere, and then they sit there and they grow.

I think that in a similar way, products and narratives have this relationship to each other. Once a product exists, a lot of narrative forms around the product, and the product changes that narrative, and the narrative changes the product. So they're both important. Just like a sperm and an egg, or a mitochondria and a cell—they both depend on each other to keep propagating.

But I do think that today, on the margin, we're missing more product than we are missing narrative. Or at least maybe it's just people I know. Maybe just having been in academia and having lots of intellectual friends, I think there's a lot of people generating narrative and we could be generating products instead. I think we should all be learning how to do that faster, possibly with AI as a tutor to help us be better product managers or better engineers. So when I say narrative is not important, or when I say product is more important, I just mean it's more neglected right now.

[00:41:31] Beatrice: It's interesting because I don't feel like that's what I am hearing. Probably because of my selection bias in working at the Existential Hope Program, but people are telling me that we're lacking narrative. Like a positive narrative. Especially from people in academia, I hear that there are no visions for how the future could go well. But this is not your experience?

[00:41:58] Andrew: So, we're sort of lacking a narrative in a trivial sense: there is no narrative so powerful—no positive narrative—that is so powerful on its own that it just steers humanity into that future. But there's not going to be such a narrative, I think. But there could be a product that nurtures a narrative like that, that steers humanity.

[00:42:29] Beatrice: Yeah, I guess why I think it potentially matters with the more positive narrative is that currently in mainstream culture, it feels like... I think the statistics I heard of which percentage of young people think that they're going to get a better life than their parents is like 40% in the US, which is extremely low. In France, it was like 9%. It's a very big lack of belief that the future is going to be good. If everyone thinks that this is the case, it just probably leads to this lack of agency—lack of actually doing these things that could create that better future because you don't even think it's worth it.

[00:43:19] Andrew: I agree that people are sad. There's a question of: do you solve that sadness by inserting a new narrative, or do you solve it by inserting ten or a thousand new products? I think it's the second one.

[00:43:36] Beatrice: If they're good products, I guess. Especially if they help change the situation for the better.

[00:43:43] Andrew: Like solar energy. So good. I think instead of stressing about how there's not enough of a narrative around solar energy, we could just go make solar panels. I know people who do that and I think they're contributing. We could have "narratives about narratives" and "not enough narratives about the narrative narratives," or we could just make some really cheap solar panels and spend our time in a garage making a really cheap solar panel.

Until you've done it... And people can do that. I'm not that person—not this year, and probably not this decade. But some people are. There is more to it; you have to sell the product and the narrative helps you sell it. But I think the product has to be there first. I feel that's more missing in society. So if anything, I'm trying to make a counter-narrative, which is: if you're finding yourself preoccupied with changing the narrative, stop. Make a product instead, and then use the product to create the narrative you want.

[00:44:48] Beatrice: This is just a narrative itself, which I acknowledge.

[00:44:52] Andrew: I feel like we have so many narratives now.

[00:44:52] Beatrice: Yeah. I think it's a great idea, but to some extent, it's just harder or scarier to actually do the product thing. And also that people might not feel... but that's what you're trying to do. You're trying to encourage more people to just do it.

[00:45:16] Andrew: Yeah. Make stuff.

[00:45:18] Beatrice: It's very like a startup culture. Do you think it's the "move fast and break things" or is it different? Because it feels like there's definitely people creating products that they will make money on, but I'm guessing what you're pitching here is: we want products that we think would actually make the world better. That's the distinction.

[00:45:37] Andrew: Yeah. For one thing, a certain subset of America and a certain subset of the world thinks that profit is bad. I think that's not good. I think it's not good to think that profit is bad.

I think if a person does a helpful thing for another person, it is good if that first person benefits from that a little bit so they can fuel themselves to do more of that same helpful thing in the future. But if every time you help, it comes at a cost to yourself, then you shrink and you can't do more of the helping. Helpful activities—goodness—needs to pay for itself so that it can grow and do more goodness.

Evil can feed itself sometimes and can grow, so it's not that profit automatically prevents evil. But profit is not evil. If we're going to deal with the level of narratives, I think there's too much of an anti-capitalist, anti-product, anti-profit narrative—certainly in California, which is interesting because California is extremely productive and industrious. I would like to see more positive "Hey, let's make good things. Let's just make 'em."

And you don't have to make one good thing that fixes everything. Like the person who made these headphones... or the ten or a hundred people who invented these things, they helped me. They help me every day. Every day I'm trying to do something good in my job or my personal life that requires me to concentrate. It could be a family member's feelings that I need to think about and I need some quiet time, or it could mean a paper I'm writing or code I'm writing. These help me. So I'm a better person—I do better—because of these. If I was a bad person, they would help me be a better bad person. So it's not like these can't be used for evil. We could have the inventors of these headphones going around feeling guilt about all the evil people that they gave earmuffs to. But I think probably overall they helped, and I'm really grateful that they helped me. I think we can make more things like that instead of being paralyzed about making the very best thing all the time.

[00:47:58] Beatrice: And the best way to identify the best products is just to think about what are the problems that we're trying to solve.

[00:48:05] Andrew: You just did it. You just said, "What's the best way to identify the best products?" Why does it have to be the best way? Why does the product have to be the best? Like, is this water bottle better or worse than these earmuffs? Which one is the best product?

[00:48:25] Beatrice: Depends on what you need.

[00:48:27] Andrew: Well, I think they're just both good. And I didn't talk about the water bottle, but it's also quite good. Fixation on "Is this the best thing?" is really paralytic. I'm not saying that you're paralyzed, but many people are paralyzed by that word "best." It's better to just think... let's talk about better. You see how I'm talking about what's better? What's better than best is better.

[00:48:55] Beatrice: Okay. Well, I do think to some extent I'm paralyzed by it. Not as much as some people for sure. It's actually quite a relief to take that load off. So, good point. I'll give you that.

If we take it back a little bit now to our Existential Hope / AGI futures... what do you think are a few characteristics that you would like to see in an AGI? What's your Existential Hope vision of our future with AGI?

[00:49:42] Andrew: Instead of a vision, which is just one future that's maybe the best or my favorite, I instead want to talk about some principles I want to push more on. There are some things everyone's already pushing on that I want to push on with everybody. The honesty, helpfulness, harmlessness, and AI transparency in the industry I think is great. So I just want to say "Yes." It's not like nobody's pushing, but more is good.

I'm not as excited about regulations that ban things, other than banning opaque things. I really think AI companies are doing pretty good work right now. They're getting better. They're all a little shy about their intellectual property and they need to defend it a certain amount, but there are kinds of transparency into their operations that we can demand that would probably accelerate the whole industry actually—accelerate and ameliorate the whole industry—so that the industry is doing more good, more quickly. So transparency is a big one.

And then something that I think nobody's talking about... I'll now go into weird stuff that I think about, but it shouldn't be weird: De-escalatory self-defense.

[00:51:02] Beatrice: Okay. What's that?

[00:51:05] Andrew: There are all these ways in which people and entities have to defend themselves—individuals, countries, companies. You have these AI companies that are suing each other or getting sued. There are legal attacks and legal defenses. Culturally, people get canceled or attacked on the internet. That's a kind of thing that people feel like they need to defend themselves against. So there are political attacks, all different kinds of attacks. I'm interested in all of them. Anything that you'd consider an attack and then a defense against that kind of attack in any domain.

In international relations, there's this concept of retorsion, which is like watered-down revenge where something bad happens and then you just respond with a counter-attack, but it's smaller. It doesn't have to be as big as the first one. It just has to be enough to make it not worth it for the counterparty.

If someone hurts you by 10 and you hurt them back by 1, well, that hurt for them. They don't want to do that again. It hurt them by one point. The fact that that's an effective deterrent is really not talked about enough. I wish everybody realized that there are ways of defending yourself that are de-escalatory and that humans can understand this. Countries, companies, AIs can understand it. I honestly think that if that cultural principle of de-escalatory self-defense were more common, we'd see less culture wars. We'd see less likelihood of an existential conflict between humans and AI. Actually, I think we'd see a less likely human extinction event.

I do think that there's a kind of cultural choice that all the AI labs are making about how much to promote this or similar ideas of peace and harmony that are not totally pacifist. It's not totally "turn the other cheek"—it is to strike back with a 1 in response to a 10.

On the margin, at the time of the New Testament being written, the Old Testament was like "an eye for an eye." There was this really harsh idea that you strike back as hard as you were struck. And then the pendulum swung the other way, which is like, "No, if someone hits you, just turn your cheek so they can hit you again." I think that's not quite right either. And then you see Islam swinging back with the beheadings of enemies and things. I think there's this thing in the middle where you're actually supposed to strike back. You're supposed to defend yourself, but you're not supposed to escalate unnecessarily.

That's how the conflict can sort of wind down. If everybody were more actively on the lookout for retorsion—it's called a retort, in lieu of revenge—I think that society would coordinate better.

[00:53:54] Beatrice: Yeah, I love that idea. Actually, I also hadn't heard that phrase before: De-escalatory self-defense.

[00:53:59] Andrew: Well, "retort" is a very common phrase. It's well-studied. And there's another one that goes well with it that isn't talked about as much in international relations, which is called disgorgement.

Disgorgement means taking away the benefit, taking away ill-gotten gains. So if someone robs your house, they should not only be punished a little bit for the robbery, but they should totally not be allowed to keep any of the stuff they stole.

Here's a little story I like to tell to motivate this. Let's say someone comes to your lawn and likes a certain plant that you have on your lawn, and they just tear up the plant and take it over to their lawn. That was theft. Now, maybe they thought it was their lawn, or it was community property, or maybe they don't understand something. Maybe the police are busy; you can't really count on the police or something. Or you're in a rural area with no police, like where I grew up.

I think the first thing you should do is look for a mutually beneficial trade. First, don't go to revenge. Say, "Hey, that was my plant. Can you pay me for it? If you pay me $200 for that plant, that's a win for me. Do you want it bad enough to pay me 200 bucks?" They might just say yes. They might say, "I'm sorry, I didn't realize it was your plant and I do really want it. Here's $200. Just get a neighbor to verify that really is your lawn." That's the best outcome because now you both got something more than what you were expecting.

So first go for a win-win. In the case of a transgression like that, try and find a win-win. If that fails—if they're like, "No, I don't want it for 200 bucks"—there's a second best option, which is restoration. They could just give it back to you. They might agree. They might think, "Oh, I'm sorry." Or they might cause you to realize it wasn't your lawn. They might say, "Actually, did you know that's not your lawn? Check out this map."

But anyway, you might get restoration of justice there, and that's the second best thing. But you should only go for that restoration after looking for the win-win. People don't do that; they just get angry. So first look for the win, then go for the restoration.

And then if restoration doesn't work—where you can't get it back or they're not going to give it back—then you can destroy the plant. That's not to say destroy the rest of their lawn. I don't think that's good, but you can destroy the plant. That way they learn that if they take plants from that area, they don't really get to keep the plant, so it's not worth their time. That's called disgorgement. It's where you, or whatever the neighborhood thinks, decides that it was not fair for them to benefit in that way. So you destroy the benefit.

And still, we're not at revenge territory because you're not making them worse off than they started. You're just restoring them to their earlier state. You're not recouping the plant, but you're able to just make it not worth it for them to keep invading that territory.

You can add a little bit of retorsion—just to make sure that it was overall an inconvenience for them to have invaded your territory. But revenge is not only the last resort, it's basically just never worth it. You don't need to hurt someone as badly as they hurt you for it to not be worth it to them. It's just not necessary.

[00:57:49] Beatrice: The reason that—putting aside that revenge often happens for very rational or emotional reasons—the reason the other things aren't happening is because they're extremely coordination heavy. You have to have the time and energy to think about good strategies. Are you familiar with any good AI products helping with this now? Like the coordination challenges?

[00:58:17] Andrew: You could write a mediation tool that's like, "Hey, we have a problem. Let's talk to this mediator." And it'll try and get us the win-win. And if that fails, it'll try and get us the restoration. And if that fails, it'll try and get us the disgorgement, and then we'll have a boundary—a little bit of scorched earth between us that's been destroyed—but at least we won't have a repeat.

[00:58:36] Beatrice: I wanted to get back to one question I asked you earlier that I feel like I didn't do a good job of following up on, which is the succession point. We never really covered that. I think we covered that you are not a fan of succession, but do you want to expand a bit more on why you think that's potentially bad?

[00:58:57] Andrew: Yeah. I do think that AI can be quite good and can be better than humans in many ways—maybe happier and kinder and things like that. So I'm not saying that AI can't be better than humans in a lot of ways. But that should somehow fundamentally devalue or eliminate humans? That also doesn't seem right.

I know people who are much smarter than me and kinder than me, and I don't want to die. And they don't want me to die because they're smart and kind. I think we would both agree it's a mistake for them to wish death upon me for that. And so I don't think AI should wish death upon humanity just for being smarter than us.

[00:59:39] Beatrice: Yeah.

[00:59:43] Andrew: It could happen. I'm not saying it won't. In fact, I'm quite worried that would happen. But it shouldn't.

[00:59:49] Beatrice: The current time is a very good opportunity to try and make it so that we have very kind AI systems that will actually be revolutionizing in terms of how good the world could be. I was thinking of starting to wrap up, but is there anything you think that we haven't covered or a tangent that you want to go on?

[01:00:16] Andrew: I really want to emphasize that having realized myself that I think products are really important for improving culture, I really also feel nascent in that understanding. I think there are people much better than me at product development and at shipping good, helpful things in the world. I wish that more of the culture of worry about AI was more oriented on learning from those people.

[01:00:45] Beatrice: Is the structure that you had to your career—doing a lot of thinking for the first years and now working on building—something you would recommend? Or do you think you should just go straight into building?

[01:01:01] Andrew: I think people should try and build things first that help themselves. Try and build something to help you with whatever you need. And if it helps you, build it for other people. Maybe it'll help them too; maybe you'll have to change it a little bit for them. But I think it's a good start for a lot of people.

[01:01:17] Beatrice: But I was also thinking about how you spent the first decades just thinking. That must give you a very useful perspective on many things that maybe if you just go straight into building when you're very young, you might miss.

[01:01:38] Andrew: I really don't know. I think if I already considered myself an expert products manager, then I would maybe have an answer to the question. But I don't know yet. Because I think the answer is either: "Don't worry about it, just build stuff and the world will give you feedback and you'll do great." Or the answer is: "Know that the process is really fraught and you need a certain philosophy in order to do that well."

And if number two is the answer, I don't know what the philosophy is.

[01:02:12] Beatrice: Yeah. Well, is there anything else you want to share just in terms of existential hope or hopeful futures before we wrap up?

[01:02:23] Andrew: There's going to be lots of AIs and humans doing stuff together. Let's do good stuff together.

[01:02:28] Beatrice: That's great. And yeah, I think the "shipping products and just putting out more of the culture that you want to see in the world" is a very clear main takeaway from this conversation.

[01:02:42] Andrew: Yeah. Thank you.

[01:02:44] Beatrice: Thank you so much.