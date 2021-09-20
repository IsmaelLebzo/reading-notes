# REST

![image](https://static01.nyt.com/images/2016/02/28/magazine/28mag-teams1/28mag-teams1-superJumbo.jpg?quality=90&auto=webp)

## What Google Learned From Its Quest to Build the Perfect Team

Julia Rozovsky, like most 25-year-olds, had no idea what she wanted to accomplish with her life. She had previously worked for a consulting business, but it was not a good fit for her. Then she went to Harvard to work as a researcher for two professors, which was intriguing but lonely. Perhaps working for a large business would be a better fit. Perhaps a rapidly expanding start-up. All she knew was that she wanted to work in a more sociable environment. "I wanted to be a part of a community, something that people were creating together," she explained. She considered a variety of options — Internet startups, a Ph.D. degree — but nothing felt quite right.

When Rozovsky came on campus, she was placed in a study group that the school had deliberately designed to create close connections. Study groups have become a rite of passage for M.B.A. students, a method for them to experience working in groups and a reflection of the growing demand for employees who can negotiate group dynamics deftly. Today's worker could start the day by cooperating with a team of engineers, then send emails to colleagues promoting a new brand, then hop on a conference call designing a whole other product line, all while juggling team meetings with accountants and the party-planning committee.

As a result, Rozovsky began seeking for new groups to join. Some students, according to a classmate, were forming teams for "case competitions," events in which participants offered solutions to real-world business issues, which were judged and rewarded with trophies and cash. Although the contests were optional, the labor was similar to what Rozovsky and her study group did: performing extensive research and financial analysis, producing reports, and delivering presentations.

Our data-driven era allows us to scrutinize our work habits and workplace idiosyncrasies in ways that our cubicle-bound forefathers could only imagine. Psychologists, sociologists, and statisticians are examining everything from team composition to email habits on corporate campuses and in university laboratories today in attempt to find out how to make employees quicker, better, and more productive versions of themselves. "We're in the midst of a golden era of personal production," says Marshall Van Alstyne, a Boston University professor who studies how individuals exchange knowledge.

THE WORK ISSUE: REIMAGINING THE OFFICE:

1. How to Build a Perfect Team
2. The War on Meetings
3. The Case for Blind Hiring
4. Failure to Lunch
5. The 'Good Jobs' Gamble
6. Rethinking the Work-Life Equation
7. The Rise of White-Collar Automation
8. The Post-Cubicle Office
9. The New Dream Jobs

The technology sector is not only one of our economy's fastest-growing segments; it is also becoming the world's dominating commercial culture. And certain self-mythologies and dictums lie at the heart of Silicon Valley: everything is different now, data rules supreme, and today's victors deserve to win because they are clear-eyed enough to dismiss yesterday's conventional wisdoms in favor of the disruptive and novel.

# A Conversation about REST

Brother: Hello, I'd like to ask you a question... What is the identity of "Roy Fielding"?

ME: He's a weirdo. He's clever.

Brother: Oh, really? What exactly did he do?

ME: He was a key contributor to the development of the first web servers, which transmitted documents over the internet... Then he spent a lot of time researching why the web functions the way it does. His name appears in the protocol specification for getting pages from servers to your browser.

Brother: Isn't a website a resource?

ME: Sort of. A web page is a resource's "representation." Resources are only ideas. URLs are the addresses that you put into your browser...

Brother: I'm familiar with the concept of a URL.

ME: Without a doubt. Those URLs inform the browser that an idea exists someplace. After that, a browser might request a particular representation of the idea. The browser specifically requests the concept's web page representation.

ME: In any case, HTTP—the protocol that Fielding and his colleagues invented—is all about putting verbs in front of nouns. When you go to a web page, for example, your browser does an HTTP GET on the URL you entered in, and a web page is returned.

Isn't it true that most web pages have images? Those are two different resources. The web page simply specifies the image URLs, and the browser does more GETs using the HTTP protocol until all of the resources have been received and the web page has been displayed. But the essential point to remember is that nouns of quite diverse types can be treated in the same way. It doesn't matter if the noun is a picture, text, video, mp3, slideshow, or anything else. Given a URL, I can GET all of those items in the same way.

Brother: So, for all of their pages, individuals would have to develop machine formats?

ME: If it were worthwhile.

Let's face it, we've been talking about this in a really abstract way. Let's look at a real-life scenario. Consider yourself a teacher: at school, you presumably have a large computer system, or three or four, that allows you to manage students: what courses they're in, what grades they're getting, emergency contacts, information on the books you teach from, and so on. If the systems are web-based, each of the nouns involved in this case is likely to have a URL: student, instructor, class, book, room, and so on. Getting the URL using the browser currently returns a web page.

Because all of that information would be consumable in a standard way if each URL had a machine readable representation, adding additional tools to the system would be simple. It would also make it much easy for each of the systems to communicate with one another. You might also create a state- or country-wide system that could communicate with local school districts to collect test results. The options are limitless.
