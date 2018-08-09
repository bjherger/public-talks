# Lit review

## Resources

 - [cheat sheet](cheat_sheet/scrum_cheat_sheet.md)
 - Agile quick reference book
 - Retro book
 - [Atlassian Retro playbook](https://www.atlassian.com/team-playbook/plays/retrospective)

# Outline

 - Intro / Why scrum
 - What is scrum?
 - Cheat sheet

Follow up blog post:

 - Roles, Meetings & artifacts

# Draft

## Title

Project Management, for Data Science

## Content

Managing Data Science projects is a unique proposition. Data engineering and modeling can be more iterative and open ended than most realms of software engineering and varying data quality can cause huge changes in the level of effort necessary to train a model. 

This begs the question: 'How do I keep Data Science projects rolling?'. In my work delivering fraud, cyber security and natural language processing projects at a Fortune 100 company, I've found Scrum to be an invaluable paradigm for scoping and delivering data products. It's also a paradigm shift for many Data Scientists, so let's dive a bit deeper into what Scrum is, and how to make it work for you. 

### What is Scrum?

Scrum is a set of roles, meetings and artifacts that allow teams to work happily and effectively. This paradigm has been developed and optimized by companies like Google, Tesla, Apple and Salesforce to:

 - Minimize meeting time
 - Regularize workload
 - Keep projects tightly tied to customer need

We'll dive deeper into the Scrum paradigm in Part 2, and for now, I'll focus instead on the high-level goals of the paradigm, and give an in-depth intro in a future blog post. If you want a sneak peek, [many](https://www.youtube.com/watch?v=9TycLR0TqFA) [great](https://www.atlassian.com/agile/scrum) [introductions](https://www.scrum.org/resources/introduction-scrum) to Scrum are available,

A core principle of Scrum is to iteratively improve a product, identify feedback, and scope out future improvements. This avoids 
building needless features ([clippy](https://en.wikipedia.org/wiki/Office_Assistant)) or getting too attached to an inefficient workflow. 

Additionally, the atomic unit of time in Scrum is a sprint (usually 1, 2, 3 or 4 weeks). This atomic unit of time allows teams to iterate rapidly, minimize meetings, and still have regular time to work through items that are slowing the team down. During each sprint a team will:

 - Produce an atomic, documented and integratable unit of work
 - Hold one planning meeting and one recap meeting

Let's dive deeper, and look at how to make the Scrum paradigm work for you. 

### Customizing the Scrum method

Scrum is a paradigm that has been found helpful at many companies, but the dirty secret is that each of these shops have iterated on and customized the Scrum paradigm for their domain.

While no two teams are the same, there are a few tips and tricks that I've found helpful for running Scrum on Data Science teams. 


#### Start with a bang

Give the team context. Let them know why your organization is investing Scrum, the benefits of Scrum, and how long you expect the learning curve to be.

 - Yes: Have a kick off meeting, and let people know that there will be a learning curve.
 - No: Expect that the team will immediately 'get it', or that they will be as productive while learning a new project management style


#### Make milestones tangible

Data Science is often an iterative process, with unknown data issues lurking at every step. This is an opportunity to focus on tasks, rather than results when laying out milestones. 

 - Yes: Create tangible milestones, such as `train a baseline model`.
 - No: Define milestones with a large possible time range, such as `train a model with .98 test AUC`.


#### Explicitly address data quality

Variable data quality is an issue that is unique to Data Science and doesn't affect other realms of Software Engineering in quite the same way. It's helpful to allocate a bit of extra effort to adress this. 

 - Yes: Create tasks specific to data QA, and building POC models to gain domain experience, such as `Evaluate schema and nulls of sales data set`, or `build a prototype transformation pipeline, to inform final pipeline design`
 - No: Roll data QA into other tasks, such as `Gain access to data set *and* build baseline model`

#### Communicate uncertainty

Additionally, Data Science's highly iterative process makes nailing down deliverables and delivery dates difficult. Rather than a weakness, I've turned this iterative process into a strength, by using each iteration to fold in client feedback.

I'd highly recommend bringing clients into the feedback loop, to help tailor future work

 - Yes: Get regular feedback and guidance from clients with tasks such as `Provide v0.3 model to policy maker, get feedback on what works well`, and or `Get partner feedback on current stable of models, to inform future iterations`
 - No: Build long term, immovable project plans, or create stacks of tasks that rely on each other and could become derailed. 

