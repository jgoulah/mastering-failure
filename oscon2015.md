build-lists: true
# Building A Successful Organization By Mastering Failure

### John Goulah
### Etsy

---

![](images/etsy_logo_lg_rgb.png)

^ A marketplace for people around the world to connect, buy, and sell unique goods 

^ Etsy is the marketplace that we all make together, and our mission is to re-imagine commerce in ways that build a more fulfilling and lasting world

---

# Marketplace

- $1.93B Annual GMS 2014
- 1.4M active sellers
- 20M+ active buyers
- 30% international GMS
- 57%+ mobile visits

---

# Infrastructure

- over 5500 MySQL databases
- 750K graphite metrics/min
- 35K nagios service checks
- 1.3GB logs written/min
- 30-50 deploys / day

---

# Company

- Headquartered in Brooklyn
- Over 700 employees
- 7 offices around the world
- 80+ dogs

---

# Values

^ we are a values driven company

---

![fit](images/mission-values-culture.jpg)

^ values are our path towards the mission, and everything is surrounded by the culture

<!---

# Company Values

- We are a mindful, transparent, and humane business
- We plan and build for the long term
- We value craftmanship in all we make
- We believe fun should be part of everything we do
- We keep it real, always
-->

<!-- good notes here: https://jira.etsycorp.com/confluence/display/COM/Communicating+in+Ways+that+Align+with+Etsy's+Values -->

---

# Learning Org

a company that facilitates the learning of its members and continuously transforms itself

^ concept was coined through the work and research of Peter Senge and his colleagues ; encourages more interconnected way of thinking

---

# Five Disciplines

^ Senge is a systems scientist who is a sr lecturer at MIT and founder of the Society for Organizational Learning

^ Author of book The Fifth Discipline: The Art and Practice of the Learning Organization.

^ Senge popularized the concept of the learning organization through his book The Fifth Discipline. In the book, he proposed the following five disciplines

---

# Systems Thinking 

process of understanding how people, structure, and processes influence one another within a larger system

^ Organizations are a system of interrelationships. To become more successful we need to analyze these relationships and find the problems in them. This will allow an organization to eliminate the obstacles to learning

^ But important to view  "problems" as parts of an overall system, rather than reacting to specific parts, outcomes or events, and thereby potentially contributing to further development of unintended consequences.

---

# Personal Mastery 

an individual holds great importance in a learning organization.

^ Continuous self-improvement holds as much importance as commitment and work for the organization. Employees need to grow and work on their own goals.

---

# Mental Models 

the assumptions held by individials and organizations.

^ This is the company culture and the diverse theories and mindsets that serve as a framework for the functioning of the organization. Learning organizations look for how these affect organizational development.

^ important to replace confrontational attitudes with an open culture that promotes inquiry and trust


---

# Shared Vision 

creates a common identity that provides focus and energy for learning.

^ A learning organization's employees all share a common vision. Personal goals must be in sync with the goals and vision of the organization.

^ The most successful visions build on the individual visions of the employees at all levels of the organization

---

# Team Learning 

the problem solving capacity of the organization is improved through better access to knowledge and expertise.

^ Requires individuals to engage in dialogue and group discussion. For a team to learn, they must be in sync and reach agreement.

^ Therefore team members must develop open communication, shared meaning, and shared understanding.

---

# Learning About Failure

- architecture reviews
- operability reviews
- blameless post mortems

---

# failure and success come from the same source

^ they come from the same source,  ordinary work, only difference in failure
things have come together in unexpected way

^ some of the things that I listed as learning tools such as arch/op reviews, failure hasn't yet happened

---

![](images/faces.jpg)

# context

^ some alignment of random variables in the system causes context to change

---

# can study the system at any time

^ if field experts study the system, you can find the same things you would in a postmortem

---

# three inflection points

- architecture reviews
    - early feedback and discussion
- operability reviews
    - hold before launching
- blameless post mortems
    - hold after a failure

---

# Architecture Reviews

---

# Architecture Reviews

understand the costs and benefits of a proposed solution, and discuss alternatives

---

# Etsy Tech Axioms

- we use a small number of well known tools. 
- all technology decisions come with trade offs. With new technology, many of those trade offs are unknown.
- we’re growing. things change.

^ have to show our tech axioms to get understanding of why we examine new methods and departures 

---

# [fit] with new technology

# [fit] many of those tradeoffs are unknown

^ we want to examine these tradeoffs

---

# Departures

a departure is when new technologies or patterns are introduced that deviate from the current known methods of operating the system and maintaining the software

^ we call these new technologies departures

^ this includes new languages, new database systems, or a new templating pattern

---

# How do I know I need an architecture review?

when there is a perceived departure from current technology choices or patterns

^ in other words some new tech we don't have experience with

---

# How early do you hold them?

early enough to be able to bail out or make major course corrections

---

# Who should come?

- the people presenting the change
- key stakeholders (sr. engineers, or arch review working group)
- everyone else that wants to learn about the proposed changes to the system

---

# [fit] Meeting Format

^ now lets talk about the format and expectations


---

# Preparation

- a proposal is written in a shared document and circulated
- comments are added, discussed, and potentially resolved in advance
- initial questions for the meeting are collected in a tool such as google moderator

^ some work done to avoid the longest meeting ever...

^ proposal should cover goals, mapping design onto goals, departures from existing tech, alternatives and why they weren't used, costs and pain points

---

# Some General Questions

- Do we understand the costs of this departure?  
- Have we asked hard questions about trade-offs?
- What will this prohibit us from doing in the future?

---

# Some Questions (cont)

- Are we impacting visibility, measurability, debuggability and other operability concerns?
- Are we impacting testability, security, translatability, performance and other product quality concerns?
- Does it makes sense?

---

# The Arch Review

- proposal is presented to the group
- discuss questions and concerns
- decide if we are moving forward or need further discussion

---

# [fit] Wait!

# You're saying my project might not move forward?

---

#### (maybe)

---

# Why might this end a project?

- we learned through this discussion that an alternative is better
- we find goals overlap with other projects that are in progress
- we discover that it isn't worth the costs now that we have a better idea what they are

---

# At the end we should have

- detailed notes from the conversation 
- agreement on tricky components and document 
- a compilation of learnings and questions
- a decision of whether to keep going with the project, stop and rethink, or gather more information

---

# Operability Reviews

---

# Operability Reviews

Understand how could the system break, how will we know, and how will we react?

---

# When Do We Do Operability Reviews?

- After archtecture reviews in the product lifecycle, generally right before launch
- When we need to gain increased confidence for launch due to the the technology, product, or communication choices being risky
- If there's a chance you'd surprise teams that operate the software

---

# Summary of Arch vs. Op

![inline](images/kellan-tweet.png)

---



