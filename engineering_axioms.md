1. Change is constant.
This one shouldn't be too controversial. Almost everything is always changing, including the rate of change itself. We need to acknowledge not only that our ability to respond to change is crucial, but that how well we do it (time, cost, quality, reliability) is often a dimension of our competitiveness.

2. Your product is an asset, but code is a liability.
Your product solves your customer's problem(s), and therefore is your asset. The code itself is the cost of creating the asset. The more code you have, the more it needs to be read, tested, changed, and understood. This is especially relevant when you consider axiom 1. Accept new code (and dependency on external code) conservatively. The best code is code you don't have to write.

3. Duplication is less costly than premature abstraction.
Until you have a high degree of confidence that your abstraction is going to pay for itself because it solves a real, abstract problem you really do have, don't do it. Wait and learn more. Until then, repeating code can help avoid dependency, which itself makes the code easier to change independently or delete. A premature abstraction creates complexity through dependency and indirection, and can become a bottleneck to your ability to respond to change.

4. Code should be easy to delete.
Write code to be removable, which in large part is the same as saying "decoupled". For sure not all code needs to be similarly removable, but minimising dependencies, having clear boundaries via well-defined interfaces, and having a thoughtful overall system design allows parts to be removed/changed more easily. I once heard someone use the expression "code spent", as an alternative to "code written" and I love that. I like the implication that removing code is reducing future cost.

5. Existing code exerts a powerful influence.
The very fact it's there suggests it's correct and necessary. Hopefully it is, but not always. We need to maintain both the confidence to change it, and the ability to reason about whether we should. Don't let the existence of code itself create doubt that it can't be removed. As per axiom 4, it should be easy to remove, and the system design should be good enough to enable us to understand whether we still need it.

6. Accidental complexity is one of the biggest risks.
Accidental complexity is complexity that can be avoided, and occurs due to things like poor design, bad decisions, and not prioritising an appropriate level of simplicity within a system. If simplicity is not a goal, accidental complexity is more likely to occur as a system grows, and will gradually negatively affect almost everything from changing the system to even being able to understand it. The 2006 paper Out of the Tar Pit is a worthwhile read on this subject.

7. Technical excellence can be shadowed by bad personal skills.
Unless you're working completely alone, it's not just your ability to solve technical problems, to write good code, etc, that matters. To the contrary, they matter even less if you make the people around you unhappy and less productive. Just like learning to write good code, you have to learn "to people" good as well. Empathy is a big part of this, as is recognising that people are different – be caring, be understanding, help others and ask for help yourself, be nice. Be an engineer others want to work with.

8. You are not your code. Be kind to the coder, not to the code.
Code is merely a moment in time that captured what we thought we knew about something. It's not you. You may have wrote it, but since that moment (even if it was 3 minutes ago) you've grown, but the code has not. A conversation about code, good or bad, should never be personal. Keep it professional. Talk about the code, or about the problem, but don't make it about the person who wrote it. Use "we" instead of "you". Sometimes I try to pretend I wrote the code someone else wrote, which helps me avoid accidentally sounding personal.

9. Treat people who know less than you with respect and patience.
We all start somewhere, and the journey is a lot more joyful when you're surrounded by patient people who want you to succeed, rather than those who make you feel like you don't belong. If you struggle with this, it may be helpful to remember that the newbie programmer almost certainly does something better than you do – perhaps they're fluent in another language, or cook amazingly, or play a sport. Just imagine yourself in the reverse role. How would you like them to treat you, the total newbie? Again: be an engineer others want to work with.

10. The only true authority stems from knowledge, not from position.
Knowledge and understanding of the problem, the domain, the customer, are all far more important than whatever the first 3 letters on your business card are. Even if it does have a watermark. Understand how something works from first principles, build a solid understanding, and authority will follow.

11. Teaching is a form of learning in disguise.
If you think you know something, try teaching it. Often the very act of trying to explain what you know to someone else forces you to formalise your own thoughts much more clearly. Writing things down seems to have a similar effect. I've lost count of the number of times I've begun explaining something only to find I don't quite understand it as well as I thought.

12. Lift the skills of people around you, not just yourself.
A great team is never a great because of one amazing person. It's a great team because everyone challenges each other and everybody grows together. When you learn something cool, share it – help the people around you get better. As they do the same, everybody benefits and nobody gets left behind. It's also far more fun. Secondary benefit: axiom 11.

13. The longer you wait the more you'll know.
I'm still learning this and trying hard to avoid my almost default desire to decide quickly. The truth is, the longer you delay non-essential decisions the more information you'll have to lean on when the time comes to make it. Of course you can't always procrastinate a decision, but often you can, and as a minimum you should at least consider whether not knowing the answer right now is actually OK.

14. A good type system is worth its weight plus some.
Having gone backwards and forwards through various static and dynamic languages over my career, I'm currently of the opinion that a good type system is worth its overhead. A good type system shouldn't carry all that much overhead. If the type system is designed well, it can almost feel like a dynamic language (via features like inference and flow analysis) while removing a whole class of issues that the compiler can handle far better and quicker than you can. Developments like ownership in Rust are a nice example of how this has gone even further than people would have imagined years back.

15. The right team of people trumps everything else.
Having a team of people who just want to work together and build great things makes a lot of other problems easier to deal with. The word "right" here is highly subjective and contextual, but at least anecdotally, empathy, respect, and friendship have been recurring elements of great teams I've been part of.

16. Stick to boring technology, unless there's a good reason not to.
Boring tech is often older and better understood. There's battle-hardened experience of how to use it effectively, better understanding of its failure modes, and it's easier to find people and resources on how to best apply it. I really like Dan McKinley's idea of innovation tokens. You only get 3. Use them to adopt or build brand new stuff – ideally stuff that will make you better at your core competency – but any more than 3 and the risk of never reaching stability/maturity starts to grow.

17. Have the smallest team possible, but no smaller. Grow it carefully.
A play on a well-known quote, and your mileage may vary on this one. In my career so far, I've reliably seen smaller teams be more effective than larger ones. There's a balance to be found, for sure, which depends on the magnitude and complexity of the problem you're solving. That said, smaller teams benefit from less communication overhead, less room for miscommunication, and more space for everyone's voice to be heard. In a smaller team, it also feels more personal, and I feel more responsible, and I like that.

18. Rest.
I'm happy to see the gradual de-sexification of the "work all hours to be successful" attitude, and far more attention being put on mental health and well-being. It's incredibly difficult to feel happy when you don't feel rested, and it's even more difficult to do your best work when you're not feeling happy. To work at our best, we have to spend time not working. I like to think of rest as a key part of my ability to work, in the same way it is for physical exercise.

19. Don't pick a solution until you've thought of at least one more.
It's enticing and exciting when that thing clicks in your head and you realise you found a way to solve the problem. Perhaps with a trivial problem that's cool and there's really nothing more to do. However, if the problem is non-trivial or important, it's worth considering that there may be other solutions you simply haven't thought of yet.

To avoid getting carried away in the excitement of going from no solution to a solution, and simply going with the first thing that comes into your head, try to think of at least 1 more. Trying to find a second solution often forces you to think differently, and once you have two you'll be forced to consider the trade-offs in order to select one. Such contrasting trade-offs can often help frame the problem more clearly as well.

20. Have opinions, but avoid expressing them in ways that cause other people to believe you won't change them.
Expressing our beliefs and opinions is important, and we should all have the room to do that. However, there's a fine line between sharing an opinion and sounding as though you're sharing an immovable fact. In a team, it's incredibly healthy for everyone to feel like they can challenge an opinion and potentially change it, or their own.

A great piece of advice I received that helps with this is to express your beliefs along with a percentage of how sure you are. "I'm 95% sure using Visual Basic is a bad idea." Even when it's 95%, it's both an opening for someone to question the belief and create a conversation, and an opportunity for you to simply revise your sureness if new information is learned.

21. It's OK to say "I don't know" or "I need to research that before I have an answer".
Let's be honest, none of us have a clue what we're doing. You do? OK, well I don't. Our industry moves quickly, and while there's lots of new old things, there's a healthy amount of new new things as well. We're all learning every day, and not having an answer is absolutely fine. Our value is not our ability to know everything, it's our ability to learn, to find out, to answer those questions and create new ones.

I'm excited when someone tells me "I don't know" because now I know we can explore the problem together and both learn something. Don't hide it as though you're the only one who doesn't know. Often nobody knows, but your honesty just enabled everyone to join in openly and work together.

22. Writing throwaway code to explore a problem space is underrated.
It can be quicker to get it completely wrong a few times and start over than to attempt to get it right first time. Sometimes the best way to explore the problem is by screwing around very close to it and learning as much as you can.

Perhaps you don't really understand the problem space yet, but by trying a few things out you can discover stuff that high level conversations about design, or reading docs will completely miss. With the freedom to make as many mistakes as you like and throw it all away at the end, you can learn very quickly.

23. Manage state carefully.
Every program has state, but how that state is managed can make a world of difference. Poor management of state is a huge contributing factor to overall system complexity, and often occurs because it hasn't been thought about early enough, before it grew into a much worse version of the problem.

There are lots of different strategies to help, from particular approaches to handling state in a given environment, to using functional languages and/or approaches to create tighter constraints around how state can change. Whatever you do, be deliberate about how state in your system changes.

24. It's all about trade-offs.
With almost every decision you make, you're either deliberately or accidentally trading off one thing for another thing. Sometimes the trade-offs are obvious, but sometimes they are layers away from the thing we can see in front of us. Always be thinking about where the trade-offs may be if they're not immediately obvious.

A good example that comes to mind is Go. Go has a fairly poor type system (currently), and it's a tiny language. What's the trade-off? Due to its size, and limited support for fanciness, my code looks like your code and I read other people's code with less "wow, I need to rewrite this ASAP" than ever before and I feel far more productive. There's always a trade-off somewhere. Look for it and you'll be in a position to make better decisions.

25. A good design is one in which you can change your mind without changing too much code.
As per axiom 1, change is constant. That implies that we need to handle changing conditions well to succeed – not just external change that occurs around us and takes us along for the ride, but also the internal change that come from pivots, new features, scaling challenges, etc.

A good system design should accommodate, as much as possible, our need to change how we approach the problem without forcing us to start over from scratch. In other words, the fewer parts we have to change or remove (which should be easy as per axiom 4), the quicker we can move in the face of change; the better the design.
