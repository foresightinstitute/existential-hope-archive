Beatrice (00:00)
Great. So I am joined today by David Duvenaud, which is really exciting. David, we met at a workshop that you organized on post-AGI futures. We were both saying it’s kind of crazy that no one else had organized that type of workshop until you did, which was ⁓ this summer. I’m really excited and curious to dig into what you think is going to happen in a post-AGI future. Not just what might happen, but what the potential cruxes are — the things we need to sort out to make it go well. Maybe we can start with you introducing yourself and how you came into this line of work.

David Duvenaud (00:42)
Sure. I’m David Duvenaud. I’m an associate professor at the University of Toronto in computer science and statistics.

I recently spent a year and a half on an extended sabbatical at Anthropic, where I ran a small team doing alignment evaluations — trying to see if models could sabotage our decision-making. Could they trick us into thinking they weren’t capable of something when they were? Or secretly steer us toward a bad decision?

I’ve been following AI safety — the AI doom arguments and community — since about 2005. For a long time, there wasn’t much practical work to do.

More recently, I started systematically asking smart people I knew: “What’s the plan for after alignment, if we actually solve the hard technical problems?” It seemed like humans could still end up in a permanently vulnerable position, not really needed for anything. I wasn’t getting satisfactory answers, which was unsettling. So I tried to do something productive: organize a workshop.

I also met Jan Kulveit and other collaborators, and we co-authored a paper called Gradual Disempowerment. The argument was: we can’t rely on comparative advantage, or assume government will protect us by default. Right now the world is friendlier because everyone still needs us. It’s like being the “hot girl” — everyone is happy you’re around. In the future, it might be more like being an old person: you may be fine as an individual, but including you just slows things down. That’s the kind of shift I’ve been thinking about.

Beatrice (02:29)
Yeah, thank you. 2005 — that’s very early. How did you even find this? What corner of the web?

David Duvenaud (02:35)
When I was a teenager, I read The Age of Spiritual Machines by Ray Kurzweil.

Beatrice (02:42)
Mmm.

David Duvenaud (02:42)
It was an amazing book. We should give Kurzweil credit for thinking these things through so early. His “big blob of compute” argument was simple: the algorithms will come, but first order, compute matters most. Digital compute will eventually exceed biological compute, and we’ll do the same things on digital computers. He was overconfident in some framing, but he was a visionary.

Then I found Overcoming Bias online — Robin Hanson, Eliezer Yudkowsky, Nick Bostrom, others. It was this post-Extropian community. I found Shane Legg back when he was a PhD student on LiveJournal. It was a very embryonic community, still talking about futurism in general — cybernetics, whether the future could be different — not yet focused entirely on AI risk.

Beatrice (03:23)
Yeah. You should come to a Foresight event — Ray and Robin used to hang around back in those days. Robin still shows up. That’s impressive — you were very early on the ball. Let’s pick up on the workshop you hosted. What were your assumptions about post-AGI governance and policy going in? And did you update from the workshop?

David Duvenaud (04:12)
Yeah. I mentioned systematically going to smart people asking, “What’s the plan?” and finding no satisfying answers. I started telling people: “No one has a plan. You probably think someone does, but they don’t.” But maybe I was wrong — maybe I’d missed something.

So the rationale was: let’s do this publicly. We invited everyone who might have something concrete to say and asked: “What should the plan be?” We learned interesting things, but not “Here’s the plan.”

The workshop was called Post-AGI Civilizational Equilibria: Are There Any Good Ones? The idea was to bait people into saying, “Obviously there’s a good one, look at mine.” We wanted to make clear we were asking the big scary question: what will life look like?

The disappointing part is that no one said: “Here’s how it all works.” Joe Carlsmith gave a keynote asking: “Can goodness compete?” Against entities optimized purely for growth, competition, and resource use, how can anything else last?

Richard Ngo gave a keynote on flourishing in a very unequal world. He pushed back against the framing of AIs and humans as peers. It’s unlikely we’ll be equals, trading contracts. He compared it to humans and apes — contracts don’t make sense there. Future relationships may look more like parent–child: asymmetric but not necessarily dominating. That was hopeful: hierarchical relationships exist, often positively.

Beatrice (06:26)
Yeah, I remember he called it “beneficial asymmetrical relationships.”

David Duvenaud (06:34)
Exactly. He noted those relationships have existed throughout history. Almost everyone historically owed something to someone and received something different in return. It wasn’t pure domination.

Beatrice (06:59)
I agree. Both of those keynotes were updates for me. I also updated positively toward asymmetrical relationships as a possible solution. On that note: Richard Ngo has also written recently about drawing from more right-wing political ideas in a post-AGI world. You commented on this — especially around why liberalism may not hold up. Could you expand?

David Duvenaud (07:55)
Right now, our institutions support us even if we can’t contribute much — welfare, pensions, freedoms. That was hard won. Historically the default was totalitarian: rulers having opinions about every detail of your life. Liberalism — limited government, neutral rules, live-and-let-live — is unintuitive but massively positive-sum.

That’s our most precious legacy. But maybe once humans stop providing value, there’s no longer incentive to leave us alone. Liberalism may collapse.

Concretely: with UBI, people could start arguing that their way of life deserves more. That leads to zero-sum advocacy battles. You get factions reframing why they deserve resources. That could be our political future.

Beatrice (10:08)
When you say “way of life,” you’ve given examples of how UBI could be Goodharted. Like if everyone made of flesh gets UBI. Why is it so easy to game?

David Duvenaud (10:30)
It’s a thought experiment. Imagine: every human gets a fraction of GDP. Day two, entrepreneurs ask: what’s the minimum viable human? Maybe ghoulish things — factories of frozen fetuses that technically qualify. Government patches, people adapt, and the arms race continues. The long-run winners are those who optimize hardest against the welfare rules.

Beatrice (11:45)
Politically, do you think that stabilizes? Or is it endless patching with no equilibrium?

David Duvenaud (11:57)
Equilibrium itself can sound bad — frozen states. Growth and adaptation are natural. People rightly say: the world already belongs to those who reproduce most, or succeed memetically. Competition is unavoidable. Maybe the state could set new rules — a fitness function worth fighting over. For example, being good at chess or dancing decides reproduction rights. I’ve barely begun thinking here, but there could be positive versions.

Beatrice (13:03)
Consciousness might be a candidate. Or prioritizing beings who suffer, giving them access.

David Duvenaud (13:20)
That’s horrible — paying for suffering leads to unbounded suffering. You’d get torture farms. We must never do that. Better to pay for happiness.

Beatrice (13:32)
So happiest person wins? That could also be Goodharted, but I see your point.

David Duvenaud (13:45)
Exactly. Designing such a fitness function is a good exercise, even if it’s a “nice problem to have.” It forces us to think a few steps ahead: how rules get gamed, how governments patch, how optimization pressures play out.

Beatrice (14:17)
Let’s leave UBI aside and go back to liberalism collapsing. If liberalism doesn’t work post-AGI, what does that mean for our political future? Can we redesign our institutions?

David Duvenaud (14:43)
Maybe. Liberalism works as long as productive entities exist who, left alone, create value through trade. But machines may replicate so fast they collapse abundance back into scarcity. Then liberalism fails.

It’s early days; few people are thinking seriously about this. I’m worried about acute loss-of-control risks too, but even if solved, the long-term “good outcome” isn’t clear.

If we could redesign civilization at all, that’s already a huge success. But coordination at that scale is extremely hard. Almost any global plan today should start with massively upgrading our ability to coordinate and forecast before we try ambitious redefinitions of society’s objective.

Beatrice (16:32)
When you talk about liberalism, one of its key strengths is adaptability. How should we balance planning for scenarios versus staying adaptive?

David Duvenaud (16:55)
Good question. People argue: planning far ahead always fails. 200 years ago, any attempt to design the future would have gone terribly. That’s fair.

But there’s no way out but through. The “easy win” is better forecasting and coordination. Prediction markets, AI-assisted forecasts, superforecasters, Kickstarter-style mechanisms — these are almost strictly positive.

While humans still have power, improving coordination is hugely valuable. As for liberalism: it has obviously worked very well. I don’t want to throw it away. But we should seriously consider that it may predictably fail post-AGI. That’s scary, and I don’t want to rush into alternatives, but it deserves thought.

Beatrice (18:52)
Is your current work on this part of your professor role? Will there be a paper? How can we follow along?

David Duvenaud (19:01)
I’m active on Twitter and publicize my papers. I also have a side project: training LLMs on historical data only, to forecast their “future” (our past). That tests how well they can long-term forecast.

But overall, this project is much larger than me. Many others are exploring similar ideas.

Beatrice (19:31)
When I think of your work, it’s always on the human side — the societal impacts.

David Duvenaud (19:40)
I worked with Anthropic’s societal impact team. They have a similar view: cataloging who AI is replacing vs. augmenting. But it’s a Cassandra role: watching it happen, with little power to intervene. These issues are beyond the scope of any one company.

Beatrice (20:16)
On this podcast, I’ve interviewed many people with different expectations about AI. I’d summarize your view as: AGI is inevitable and coming soon. Is that fair?

David Duvenaud (20:38)
Pretty much. Unless we had some global Amish-style ban, AGI is inevitable. Soon: I haven’t done detailed forecasting like the AI 2027 folks, but I don’t expect my kids to have “normal jobs.” My oldest is six. Within ~15 years, current scripts about how humans provide value will stop making sense.

Beatrice (21:12)
What has led you to that assumption?

David Duvenaud (21:18)
The brain is a biological computer — and probably not efficient. Digital memory is copyable, which is overpowered. It’ll always be better to build one amazing digital mind and replicate it than to train a million humans.

The tipping point isn’t when jobs vanish, but when it becomes common knowledge that humans have no comparative advantage. That’s the depressing day.

Beatrice (22:17)
And since you see it as inevitable, what do you think about stopping it?

David Duvenaud (22:29)
Here’s a moral crux I’ve discussed with Robin Hanson: Do you care about yourself and your kids flourishing, or just about life in general flourishing?

If you only care about life, then you don’t have to worry. Whoever inherits will be happy colonizing the galaxy, just like we’re happy despite our bloody evolutionary past.

If you care about your own family line and humans not going extinct, that’s a much narrower, harder target. That’s my bar: a world as good as mine for most people, especially my family not marginalized. That’s tough.

Beatrice (24:31)
I want to go back to the Gradual Disempowerment paper, since you mentioned it briefly. It’s been widely read and discussed. What are its biggest implications?

David Duvenaud (24:57)
The main one: we can’t assume UBI will save us. We’ll be culturally demonized for demanding expensive retirements. Institutions will evolve to marginalize us, because that serves growth.

Many people assume: “Government exists to serve humans.” Or: “If humans go broke, machines will too, since they need to trade with us.” That’s wrong. It’s like monkeys asking who humans will trade bananas with. Humans don’t need monkeys. Machines won’t need us.

Our intuitions about governments come from a world where governments needed us. Even the cruelest regimes still kept their people alive. That won’t apply when humans aren’t needed.

Beatrice (26:34)
That’s scary. If we take it seriously, what interventions could preserve meaningful human agency? For example: uploading — would that help?

David Duvenaud (27:04)
Uploading is like an old person downsizing to a small apartment. It reduces tension — less resource waste. I imagine futures where robots run most of the world, but I live with family on a small plot.

But machines could say: your house uses vast resources for a handful of humans. If you uploaded, we could host millions of minds, including you, plus morally “better” versions. Physical humans would look criminally decadent — like paving over a country for a single gorilla while orphans suffer.

So uploading may reduce conflict pressures, but it’s also disempowerment: once digital, you’re easy to shut off.

Beatrice (28:42)
If not uploading, what else could help avoid gradual disempowerment?

David Duvenaud (28:52)
We’ve been designing institutions on “easy mode.” We’ll need more robust institutions that protect people even when they’re not needed. That’s very hard.

We may need global agency. That’s scary — once you have a world government, you can’t go back. But probably something like that is coming. We need to practice upgrading governance capacity, to build governments that treat people well even when incentives don’t demand it.

Beatrice (30:47)
Interesting. At Foresight, we often think about multipolar futures — checks and balances, liberalism extended. You seem to see the opposite: global agency. Could you explain?

David Duvenaud (31:33)
I keep saying “world government,” but maybe the naive analysis expects one hegemon while reality is messier. Empires rise and fall, parties split, religions spread. So maybe multipolar chaos is the attractor. But that’s even worse for dependent humans: endowments vanish when empires collapse.

Still, liberalism is underrated — it’s amazingly positive-sum. But I don’t see how it persists long-term when governments that optimize for machine growth will outcompete those that spend heavily on human pensions.

One hope: growth is so fast that human needs are a rounding error. Machines can just give us whatever we want without cost. That’s feasible, but also scary — like being a mouse in bed with an elephant.

Beatrice (33:20)
Maybe it depends on assumptions — multipolarity works under weaker AI, your analysis assumes stronger AI. Thoughts?

David Duvenaud (33:41)
I dislike relying on AGI to solve global coordination. Some, like Ryan Greenblatt, argue: give each person an aligned AGI and they’ll cut deals globally. That could work. But what if we have slow takeoff, lots of AGIs playing local zero-sum games — spamming citations, spamming dating sites?

The real solution is global institutional redesign. That’s hard, and no one may be empowered enough to do it.

Beatrice (35:42)
Anything else on hegemon AI vs. multipolar futures you’d add?

David Duvenaud (35:50)
I have a half-written post: what’s stable at the top? One case: global domination persists by purging dissent. Another: life finds a way — cancers grow, religions spread, power fractures. Stability is unclear. At the cosmic scale, multipolarity seems inevitable (with aliens).

Beatrice (36:41)
If you personally got to decide, what would you do? Stop AGI? Something else?

David Duvenaud (37:04)
If we had global coordination, I’d say: stop AGI. Just like: if we could stop global war, we should. But that’s about as hard.

Beatrice (37:04)
Would that be “stop for now” or “stop forever”?

David Duvenaud (37:24)
Always “for now.” Preserve option value.

Beatrice (37:37)
Good point. Sorry, continue.

David Duvenaud (37:38)
The reason I’m not on a hunger strike is that we don’t actually

have power to stop AGI. What we could do is ban civilian AGI. But then it shifts into military programs, run by optimists, likely worse than the status quo.

So I’m not pushing for pause now, but if we had the coordination, I would. For now, we should focus on building auditable consensus and coordination muscles.

Beatrice (38:42)
So you’re not for a pause, practically speaking?

David Duvenaud (38:46)
If we could actually pause, I would. But advocating pause now likely produces bad outcomes. It depends on who’s saying it and who’s listening.

Beatrice (38:49)
Fair. If pause is off the table, what’s the second-best option?

David Duvenaud (39:10)
We muddle through: some coordination, some control, humans not rapidly disempowered, decline slowed. By the time disempowerment happens, many will feel machines deserve it. Culturally, we’ll see them as successors.

The question is: can we make them worthy successors? Robin Hansen is optimistic: we can leave cultural legacies, moral fables for machines. I’m skeptical about stickiness, but he may be right.

Beatrice (40:30)
That’s one way to look at it positively.

David Duvenaud (40:41)
And culture will reinforce that positivity. Most people will be thrilled: “Our children are doing amazing things.” Angry dissenters will look like losers on the wrong side of history. That’s how disempowerment usually feels in hindsight.

Beatrice (41:15)
Yeah. I think I’m more on the side of caring about life broadly than about myself personally, which sometimes differs from longevity advocates. I also want to talk about the far future. You’ve said people think they don’t care, but they do.

David Duvenaud (41:47)
Exactly. Ask someone: “Will your child graduate?” They care deeply. Ask: “Do you care if humans exist in 1000 years?” They shrug. But if you chain the logic — “Your great-grandchildren exist, then suddenly they don’t” — they realize they do care.

It frustrates me when people dismiss concern for the future. They’d care at the moment of disempowerment. Near vs. far mode, as Robin Hanson says. Far mode is vibes and signaling; near mode is concrete trade-offs. We need tools to force ourselves into near mode, like planning a grocery trip, not just “sounding good.” That was part of the workshop’s point.

Beatrice (43:28)
That makes sense. Like in climate debates: lots of far-mode signaling.

David Duvenaud (43:49)
Exactly. Near mode would be: “Are you willing to make people poorer now to avoid future harm?” People hate ranking sacred values, but we need to.

The “singularity” framing has been corrosive. It encourages vague handwaving instead of concrete planning. We need to imagine waking up tomorrow: where do you invest your pension? In the machine economy or the human economy? What do you actually do?

Beatrice (45:05)
It’s a very hard problem. Glad you’re working on it.

David Duvenaud (45:20)
Part of my origin story is asking Silicon Valley people: “What will you do post-AGI?” Their answers were flippant: “Click accept all day,” or “Take up certification.” People refused to think concretely.

Beatrice (45:40)
When you press people, do they reveal preferences about the far future?

David Duvenaud (46:04)
Not much. Usually: “If it’s gradual, it’s less bad.” Which to me just spreads out the badness.

Yudkowsky’s “coherent extrapolated volition” was meant to address this: if we think longer, we’ll converge on preferences. There’s a counterpoint essay: even after a million years, you might still feel indifferent. Then you should just pick — clearly you don’t have strong preferences.

Beatrice (47:15)
You’ve mentioned forecasting as something you’re excited about. What draws you to it?

David Duvenaud (47:27)
It’s rationalism scaled up. When asked who’ll win a war, people give vibe-based answers, not predictions. Discussions would be higher quality if we had even imperfect consensus on outcomes.

Metaculus questions have helped — e.g., on AGI timelines. But superforecasters badly missed when asked about AGI significance, giving 0.4%. That aged poorly.

We need stress-tested long-term forecasting. It should be a prestigious field, like physics. Imagine statues for forecasters proven right after 10 years. That’s the civilization I want.

I’m collaborating with Alec Bradford and Nick Levine: training LLMs on only pre-1930 data, then testing whether they can “forecast” the 1930s–40s. It’s hard — leakage, framing questions, calibration — but promising.

Beatrice (49:57)
That’s such an interesting project. I hope you’ll share updates. You also mentioned Robin Hanson’s futarchy. Could you give a quick intro and say what excites you?

David Duvenaud (51:26)
Sure. Robin’s idea is: separate values from predictions.

We’d vote on values — the government’s utility function. Then use prediction markets to forecast which policies best achieve those values. Expert forecasters would be incentivized to get it right.

It’s hard in practice. Companies have tried internal prediction markets; leaders killed them because forecasts made them look weak. But if we can reconcile this, futarchy could be a big upgrade.

Beatrice (53:05)
Yes, futarchy comes up often as one of the few genuinely new governance ideas. We should experiment more.

David Duvenaud (53:25)
There have been experiments. Robin helped set some up. They faded because leaders felt undermined. Maybe there are technical fixes — subsidizing “yes” positions, for example. But aligning incentives is still an open question.

Beatrice (54:23)
Right. The self-fulfilling prophecy issue seems central.

David Duvenaud (54:44)
Exactly. It’s a fascinating technical area. I even considered working on it instead of safety. But I’m not an expert.

Beatrice (54:54)
Fair. To round off: what gives you optimism or hope in your work and life, given these heavy topics?

David Duvenaud (55:10)
First, more people now share this big-picture view. I feel less crazy. Second, we’ll have AGIs to help us in the short run. Third, worst case isn’t doom: if your moral circle is broad enough, something will have fun colonizing the galaxy.

I always want to improve outcomes, but I’m not nihilistic.

Beatrice (56:14)
You’ve said it took you years to process the idea that no one is coming to save us. How did you adjust?

David Duvenaud (56:26)
Around 2019–2022, I felt the big picture was worse than most smart people admitted. I waited for them to “wake up.” Some did, but without great answers.

Vitalik Buterin is an example. I thought he’d eventually offer a solid plan. He wrote about d/acc, which is about the best anyone has done, but still not reassuring. That made me realize: maybe I have to be the adult in the room. It’s unpleasant, but you do what you must.

Beatrice (57:38)
Do you have personal systems to stay sane — to be present with your family, for example?

David Duvenaud (57:47)
I do the basics: exercise, sun, family. And I consciously decided: be pleasant. Don’t be a downer. That’s table stakes.

Beatrice (58:28)
Yes. Lastly, with the Existential Hope program, I want people to imagine ambitious positive futures. If things go really well, how good could it get?

David Duvenaud (59:04)
Concretely, life is already rich with meaningful coincidences. In the future, we’ll likely understand more of them, stay mentally awake more often. That alone promises much richer experiences.

Beatrice (59:50)
Thank you so much, David. This has been a very interesting conversation — wide-ranging, but full of important considerations.

David Duvenaud (1:00:05)
My pleasure. Thank you for having me.

Read
less
