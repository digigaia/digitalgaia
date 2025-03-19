# Organization

## General organization concepts

- [Resources for chief technology officers, with the emphasis on startups](https://github.com/kuchin/awesome-cto) [[reddit](https://news.ycombinator.com/item?id=26284750)]

- [Your CTO Should Actually Be Technical](https://blog.southparkcommons.com/your-cto-should-actually-be-technical/) [[HN](https://news.ycombinator.com/item?id=32987094)]

- Company handbooks:
  - [Valve](https://cdn.akamai.steamstatic.com/apps/valve/Valve_NewEmployeeHandbook.pdf)
  - [GitLab](https://about.gitlab.com/handbook/) [[HN](https://news.ycombinator.com/item?id=31270407)]

- [What I learned at GitLab that I don't want to forget](https://blog.boleary.dev/what-i-learned-at-gitlab-that-i-dont-want-to-forget/) [[HN](https://news.ycombinator.com/item?id=33963614)]

- [Building Self-Managed Teams: A Case Study from Riot Games](https://codingsans.com/blog/self-managed-teams)
  [[reddit](<https://news.ycombinator.com/item?id=27207107>)]

- [Open Decision-Making](https://web.stanford.edu/\~ouster/cgi-bin/decisions.php)  (by John Ousterhout)

- [Build Systems, Not Heroes](https://vitonsky.net/blog/2024/10/11/system-approach/) [[reddit](https://www.reddit.com/r/programming/comments/1g1e1x3/build_systems_not_heroes/)]

- [How to Build Anything Extremely Quickly](https://learnhowtolearn.org/how-to-build-extremely-quickly/) [[HN](https://news.ycombinator.com/item?id=41148517)]

- [My key takeaways from The Pragmatic Programmer](https://arkadiuszchmura.com/posts/my-key-takeaways-from-the-pragmatic-programmer/)

- book on how to run a successful free software project: [Producing Open Source Software](https://producingoss.com/)

- [High performance individuals and teams](https://pablasso.com/high-performance-individuals-and-teams/) [[HN](https://news.ycombinator.com/item?id=31532878)]

- [Software and Anarchy](https://applied-langua.ge/software-and-anarchy.pdf) [[HN](https://news.ycombinator.com/item?id=33173364)] - Possibly interesting book (~50 pages) on programming as it relates to "social ecology" and "peer production"

- [Best Books For The Inquisitive Software Engineer](https://gerlacdt.github.io/posts/programming-books/)

- [7 Powers: The Foundations of Business Strategy](https://www.goodreads.com/book/show/32816087-7-powers)

### About systems thinking (TODO: remove this section?)

[A Lifetime of Systems Thinking](<https://thesystemsthinker.com/a-lifetime-of-systems-thinking/>)
[[HN](<https://news.ycombinator.com/item?id=27412750>)]

VSM, Stafford Beer, cybernetics in general
[[wikipedia](<https://en.wikipedia.org/wiki/Viable_system_model>)]

[The WOPRS Organization Model](<https://jpreston.xyz/woprs-organization-model.html>)
[[HN](<https://news.ycombinator.com/item?id=28536432>)]

[The skill of org design](<https://commoncog.com/blog/org-design-skill/>)
[[HN](<https://news.ycombinator.com/item?id=28772033>)]


## Meetings

**biweekly / monthly meetings on readings / interesting articles / potential new projects**

people should talk about 1 (or more) articles, piece of news, or brainstorming idea of
potential new/fun/interesting projects

**meetings are audio-only, we don't want webcam**

It's freer this way, less physical constraints to participate in meeting.
We can use video for slides, images, etc.

own matrix server

meetings should be biweekly 2 hours, no planning or prepared questions, just open
discussion where everyone raises whatever question is needed by them

anything goes as to what can be talked about, people are also encouraged to talk
about their recent work if they have major changes they want to share with the others.

-> no need for minutes, no one wants to write them, and no one reads them.
If anything important needs to be written, this should happen as a documentation
writing item of some sort (eg: in linear).


(sop-ref)=
## Standard Operating Procedures

improvements to software should be made using RFC-style proposals (or BIP, EIP, etc., eg: [https://github.com/fioprotocol/fips](https://github.com/fioprotocol/fips))

[How to Stop Endless Discussions](<https://candost.blog/how-to-stop-endless-discussions/>) [[HN](https://news.ycombinator.com/item?id=25622149)]

rst/markdown template should be provided containing required sections (eg: NABC, etc. see HN comments, for instance also rename "competitors" to "alternatives")

[Documenting Design Decisions using RFCs and ADRs](https://brunoscheufler.com/blog/2020-07-04-documenting-design-decisions-using-rfcs-and-adrs) [[HN](https://news.ycombinator.com/item?id=31557835)]

check Linear's [method](https://linear.app/method) for issue tracking

code review should be a daily task, and we may need to dedicate up to 20% of a day to it. About code review processes and how to make it better/easier: [code review decision fatigue](<https://tylercipriani.com/blog/2022/03/12/code-review-procrastination-and-clarity/>) ([HN](<https://news.ycombinator.com/item?id=30665319>))


## Communication

integrate some remarks/comments about the apolitical nature of the project, we also don't have a code of conduct because this is all about the technology (neutral). And yeah, we should be nice to each other, but that isn't a thing from the project, it's just good human behavior. We should operate according to [Crocker's rules](https://www.lesswrong.com/tag/crockers-rules)

also check [Kraken culture](https://kraken-culture.notion.site/) document

[Why Your ‘Harmonious’ Team Is Actually Failing](https://terriblesoftware.org/2025/03/12/why-your-harmonious-team-is-actually-failing/) [[reddit](https://www.reddit.com/r/programming/comments/1jahlkh/why_your_harmonious_team_is_actually_failing/)]


## Voting processes

collective is composed of 5 people, each 1 vote. votes are cryptographically signed.

decision is taken with majority, and everyone needs to vote. Exceptionally, a decision can be taken by only 4 members if they all agree, i.e. all 4 vote for the same resolution.

collective changes can happen and need to be voted upon

eviction of one person cannot happen with simple majority, it needs to have 4 votes.

collective has multisig authority over the main account (which main account?) (3-of-5, 4-of-5?)


## Ideal collective size

```{admonition} Conway's law
:class: seealso

Any organization that designs a system will produce a design whose structure is a copy of the organization's communication structure.
```

5 people seems to be a good number to target as it provides balance between too small a team to be more productive than a single developer and a team too big that crumbles under its communication and management overhead.

2 is too few, no diversity: just a 2-person team

3 could be, but risk of going 2 vs 1 in decision making is high and very likely resulting in the death of the structure

4 is too symmetric: it might just end up being 2 vs 2, which is 2x the case with 2 persons, which we have seen doesn't work

5 seems to not introduce too many established structures


## Similar organizations

Here are a few similar organizations / collectives that we might want to draw inspiration from:

check Framasoft, they have some pretty good ideas, tenets and organization: <https://framablog.org/>, <https://framasoft.org/en/>, <https://framasoft.org/en/manifest/>

another organization which we like and seems pretty aligned with what we want to do is [FUTO](https://futo.org/about/what-is-futo/)

[Alchemists](https://alchemists.io/): A collective devoted to the craft of software engineering where expertise is transmuted into joy.

[Trifecta Tech Foundation](https://trifectatech.org/): Open infrastructure software in the public interest

Trifecta Tech Foundation is a non-profit that develops and maintains digital commons, open-source software and open standards for vital systems.

Some "tech coops", maybe good source of inspiration
<https://tech-coops.xyz/>
