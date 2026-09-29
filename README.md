# Specification Phase Exercise

A little exercise to get started with the specification phase of the software development lifecycle. In this exercise, your team specifies a set of improvements and new features for [The Slide Machine](https://theslidemachine.com) — see the [instructions](instructions.md) for details, and the [background](background.md) for an introduction to the software product you are tasked with extending.

## Team members

- [Isha Zaheer](https://github.com/izz04)
- [Belle Mbaezue](https://github.com/nonyembaezue)
- [Sarah Toussaint](https://github.com/sarahtoussaint)
- [Scott Kim](https://github.com/jk8308-jpg)


## Review of the Current Application

- **Strength — Navigation:** The interface made it easy to understand how to create a project and start a lecture.
- **Strength — Live generation:** Slides appeared quickly while the lecture was being spoken.
- **Strength — Transcription:** The app captured much of the spoken explanation closely.
- **Strength — Slide formatting:** Generated content was usually broken into short points that were easy to scan.
- **Weakness — Seeding feedback:** Adding seed notes and seed material produced no visible result at the time, making it difficult to tell whether they had been applied.
- **Weakness — Missed speech:** When the app did not recognize certain words or phrases, it sometimes left parts of the output blank.
- **Weakness — Depth of slides:** The generated slides largely restated the spoken words without developing the explanation further.
- **Gap — Visual explanation:** In the test lectures, generated slides did not include diagrams for concepts or examples that would benefit from a drawing.
- **Weakness — Google Drive import:** An attempt to import a lecture through Google Drive could not open the file chooser; a subsequent attempt displayed an invalid developer key error.
- **Strength — PowerPoint import:** Importing a PowerPoint presentation succeeded and brought in all 96 slides.
- **Weakness — Imported slide appearance:** Some slides looked unusual after import, although it was unclear whether the cause was the app or the presentation export.
- **Weakness — Lecture creation during import:** Repeated import attempts left two empty lectures in the project.
- **Strength — Public lecture playback:** A lecture found through Discover could be opened and played back with its slides and audio narration.
- **Strength — Deck narration:** When generated slide text was unclear, a student used **Play deck aloud** to help follow the example.
- **Weakness — Finding an example:** A student had to scan through the deck to find a particular lecture example.
- **Weakness — Quiz feedback:** After an incorrect answer, the exit-ticket quiz showed the correct answer but did not explain why it was correct.
- **Weakness — Quiz wording:** A question about which part of an octopus limits the gap it can pass through was confusing because the deck mentioned both its eyes and beak.
- **Gap — Quiz-to-deck connection:** After reviewing an incorrect answer, a student manually searched the deck for the related concept; the feedback did not take them to the relevant material.

## Prior Art & Originality

See instructions. Delete this line and replace with a short statement of what your team checked (the project's Future Work and Open Questions, its roadmap, and its open issues and pull requests) and which parts of your proposal are original — new work not already specified, scheduled, or proposed by someone else.

## Stakeholders

### Instructor Interviews

#### Instructor A — Max S

Instructor A teaches technical material and has prepared lectures using brief notes, existing slides, and slides he created himself. He typically expands on his notes while speaking in class and checks student understanding through homework and quizzes.

**Goals and needs**

- Prepare lectures efficiently without building every slide from scratch.
- Teach flexibly from notes, adding explanations as the class unfolds.
- Share materials that help students review what was taught.
- Use diagrams to explain technical relationships, such as relationships between database tables.
- Find and organize relevant lectures when preparing a course.

**Problems and frustrations**

- Creating slides takes time and is the most frustrating part of lecture preparation.
- Someone else's notes or slides do not always fit his teaching approach.
- Preparation can be uneven: a topic that seemed straightforward may need more explanation during class.
- Students may expect his personal teaching notes to be complete study notes.
- Brief generated bullet points do not provide enough visual explanation for some technical lectures.

**Observations from the app session**

- He found the interface intuitive and created a project and lecture with little guidance.
- A Google Drive import attempt failed, while a PowerPoint import succeeded.
- Slides generated quickly, but the short deck from his spoken explanation lacked the diagrams he wanted.
- He would revise the generated slides before using them in class and preferred typing material over relying primarily on voice transcription.

#### Instructor B — Professor Z.

Instructor B teaches parallel computing and has taught for more than 35 years. Much of his course material comes from his teaching experience and academic papers. Because hardware and software continually change, course material can vary significantly between course editions. He adapts his lectures for undergraduate and graduate students, using more pictures with undergraduates to make complex concepts easier to absorb. He also typically uses presentation notes to expand on material during lectures.

**Goals and needs**

- Create digestible learning materials for advanced technical concepts.
- Use sophisticated graphs and diagrams to illustrate data pipelines and other complex relationships.
- Encourage active learning and participation from students.
- Adapt slides as hardware, software, course editions, and student audiences change.
- Help students understand the main ideas of a lecture rather than focusing only on what will appear on assessments.

**Problems and frustrations**

- Changes between course editions require him to revise outdated material.
- Students may focus primarily on what will be tested rather than identifying the main ideas from lecture material.
- Obtaining copyright permissions for educational diagrams can make it difficult to use certain visuals.
- Receiving answers to checkpoint questions can be difficult during class.
- Text-heavy slides are not sufficient for explaining some advanced technical concepts.

**Observations from the app session**

- He found the app useful in generating a draft for a lecture but questioned why he would use The Slide Machine instead of another GenAI tool.
- He immediately noticed the lack of pictures and emphasized the importance of students seeing visual representations rather than simply reading text.
- He observed that the app primarily transcribes audio and divides the information across slides. Although he found the transcription effective, he suggested that capturing hand gestures could potentially translate teaching actions into drawings or symbols.
- He said he would use the exit-ticket quiz feature, although he anticipated that students may not respond positively to it.

### Student Interviews

#### Student A — Ryan

Student A is a chemistry major on the pre-med track. He regularly attends science-heavy lectures and uses lecture slides and personal notes to review course material. When studying, he often returns to lecture slides to review difficult concepts and uses outside resources when the slides alone are not enough to understand a topic.

**Goals and needs**

- Review important lecture concepts efficiently after class.
- Use lecture slides together with personal notes to reinforce understanding.
- Check whether they actually understand the material through practice problems or quizzes.
- Identify concepts they do not fully understand.

**Problems and frustrations**

- Lecture slides sometimes contain only formulas or brief bullet points without enough explanation to understand the concept later.
- It can be difficult to remember the professor's full explanation when reviewing slides after class.
- Finding the relevant part of a recorded lecture can take a long time.
- Reading through lecture slides can make material feel understandable even when the student cannot actually solve related problems.
- Finding a specific concept in a long lecture deck can take time.

**Observations from the app session**

- He found the concise generated slides useful for quickly reviewing the main points of the lecture.
- He used the exit-ticket quiz to check his understanding of the material.
- After answering a question incorrectly, the quiz showed him the correct answer but did not explain why it was correct.
- He wanted to know why his answer was wrong rather than only seeing the correct answer.
- He returned to the lecture deck and manually searched for the concept related to the incorrect question.
- He wanted a more direct way to connect an incorrect quiz response to the relevant lecture material.

#### Student B — Emily

Emily is a humanities major who uses notes, assigned readings, and posted slides to review lectures and prepare written assignments. When she misses class, she relies on those materials and classmates' notes to learn what was discussed. She particularly wants to understand the examples and connections the instructor explained aloud.

**Goals and needs**

- Catch up on the main ideas and examples from a missed lecture.
- Understand how an instructor connected examples to broader concepts.
- Find a particular example when working on an assignment.
- Check her understanding after reviewing lecture material.
- See simple drawings or annotations that make examples easier to visualize.

**Problems and frustrations**

- In her other classes, posted slides may contain pictures or brief points without the discussion that gave them meaning.
- Classmates’ notes may not capture the same examples or details the instructor emphasized.
- The Slide Machine’s generated slide text was confusing in places; she needed to hear the spoken explanation to understand the enclosure example.
- She had to scan through slides to find a specific example and wished she could search for a word instead.
- The wording about the eyes and beak in the deck made the related quiz question confusing.

**Observations from the app session**

- Emily used slide 7, which summarizes the three reasons octopuses escape, to identify the lecture’s main points.
- She found the generated text about the example confusing and used **Play deck aloud** to understand what had been said.
- After scanning the slides for an example, she suggested a search bar for finding specific words.
- She hesitated on the quiz question about which body part limits the opening because the deck mentioned both the eyes and the beak.
- She said a simple “doodle” showing the octopus moving through a gap would help her understand the example.

## Product Vision Statement

The Slide Machine will help instructors turn spoken examples into reviewed visual explanations that remain with the lecture deck, so students can understand the ideas when studying later.

## User Requirements

### Instructors

1. As an instructor, I want to mark a generated slide as needing more explanation so that I can review it before sharing the deck.
2. As an instructor, I want to add a short explanation beside a slide so that students can understand a point that was only briefly summarized.
3. As an instructor, I want to connect an example I discussed aloud to its slide so that students can find the example when studying later.
4. As an instructor, I want to add a labeled drawing or diagram to an explanation so that I can show a relationship that bullet points do not convey.
5. As an instructor, I want to edit or remove an explanation and its visual so that students do not see unclear or inaccurate material.
6. As an instructor, I want to preview a slide and its explanation as a student would see them so that I can check whether they make sense together.
7. As an instructor, I want to see which slides still need my review so that I do not overlook an unfinished explanation.
8. As an instructor, I want to approve explanations individually before they appear in a shared deck so that I control what students receive.
9. As an instructor, I want to connect each exit-ticket question to the slide that supports its answer so that students can revisit the relevant material.
10. As an instructor, I want to correct or remove an incorrect question-to-slide connection so that quiz feedback does not direct students to the wrong place.
11. As an instructor, I want to add an explanation for an incorrect quiz answer so that students learn why the correct answer is right.
12. As an instructor, I want to preview the explanation and slide link that will appear in quiz feedback so that I can check them before publishing.
13. As an instructor, I want to be warned when students cannot access a linked slide so that I can fix the deck's sharing settings or publish feedback without that link.

### Students

1. As a student, I want to search within a shared lecture deck for a term so that I can find a concept without scanning every slide.
2. As a student, I want search results to take me to the matching slide so that I can review it immediately.
3. As a student, I want to search for examples as well as slide titles so that I can find something the instructor discussed aloud.
4. As a student, I want to read an instructor-reviewed explanation beside a brief slide so that I can understand the idea when studying on my own.
5. As a student, I want to see a labeled drawing or diagram with its explanation so that I can visualize how the parts of an example relate.
6. As a student, I want to know which explanation was added or approved by my instructor so that I can distinguish it from the slide's original summary.
7. As a student, I want to move from an explanation back to its slide so that I can see it in the context of the lecture.
8. As a student, I want feedback on an incorrect quiz answer to explain why the answer is correct so that I can learn from my mistake.
9. As a student, I want quiz feedback to link to the exact relevant slide so that I do not have to search the whole deck.
10. As a student, I want the linked slide to show its associated explanation and visual so that I can review the full idea in one place.
11. As a student, I want useful written feedback even when a deck link is unavailable so that I am not left with only the correct answer.
12. As a student, I want a text description of an explanatory diagram so that I can understand it if I cannot see the image clearly.

## Activity Diagrams

See instructions. Delete this line and place images of your UML Activity diagrams here, each with the text of the user story it illustrates.

## Wireframes

See instructions. Delete this line and place your wireframe diagrams here, covering every new screen and every existing screen your proposal changes, for every type of user.

## Clickable Prototype

See instructions. Delete this line and place a publicly accessible link to your clickable prototype here.

## Stakeholder Demo

See instructions. Delete this line and place a link to the deck The Slide Machine generated during your presentation here, after you have presented.

## Exit Ticket

See instructions. Delete this line and place a link to the exit-ticket quiz you generated from your demo deck and distributed to the class, along with a short note on what — if anything — you had to correct in the generated questions before publishing.
