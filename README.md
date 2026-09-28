# Specification Phase Exercise

A little exercise to get started with the specification phase of the software development lifecycle. In this exercise, your team specifies a set of improvements and new features for [The Slide Machine](https://theslidemachine.com) — see the [instructions](instructions.md) for detail, and the [background](background.md) for an introduction to the software product you are tasked with extending.

## Team members

- [Yihyun Nam](https://github.com/iindes)
- [Kathy Lin](https://github.com/lkykathy)
- [Ben Zaslavsky](https://github.com/benzaslavsky)
- [Sara Herschmann](https://github.com/saramhersch)
- [Anthony Wang](https://github.com/aw4580)

## Review of the Current Application

**Strengths**

- I introduced a personal story during the lecture, and slide machine made a slide about it even though it was not part of the original lecture outline.
- The exit-ticket quiz reflected what was actually said during the lecture, including a more niche topic
- The deck followed the lecture well
- The platform is well organized, and the controls are placed in intuitive locations. Although this was my first time using the platform, I did not need to search through multiple screens to find what I needed.
- The system accurately identified important concepts that I emphasized during my lecture. For example, when I emphasized that Python lists begin at index zero, it created a slide specifically about list indexing.
- The generated slides correctly separated major topic transitions and accurately summarized the main concepts of the lecture.
- The generated slide titles generally captured the main point of each part of the lecture, making the deck easier to understand and review.
- The exit-ticket quiz covered the major concepts that the instructor expected students to learn, even though the questions did not examine those concepts in great depth.

**Weaknesses**

- I speak really fast, so it dropped some content / could not pick it up and transcribe it
- Because again I speak fast, it didn't make slide breaks in all the correct places
- The Quiz feels a bit too AId, like I asked ChatGPT just to give me a few questions on the slide deck...
- Some useful examples and context from my spoken lecture were left out of the generated slides, so the deck captured the main ideas but not all of the useful detail from the lecture.
- Some of the exit-ticket quiz questions were repetitive and tested essentially the same concept. The quiz also focused mostly on basic recall rather than applying the concepts from the lecture.
- Slide generation sometimes lagged one or two slides behind the instructor's speech, making it unclear whether the instructor should pause and wait for the system.
- Related concepts were not always grouped correctly. In one case, four parallel concepts that should have appeared together were separated across slides.
- The formatting of equivalent concepts was inconsistent. Some concepts received separate subtitle slides while another concept at the same level did not.
- The generated transcript was sometimes inaccurate or did not align with the content shown on the corresponding slide.
- Some automatically selected images were only loosely related to the slide content and could be confusing without additional explanation.
- The slide editor did not provide enough manual control, such as reliably allowing the instructor to delete unwanted text boxes.
- Narration playback preserved the instructor's unusually long pauses and rapid speaking speed instead of presenting the content at a clear, consistent pace.
- The “Play deck aloud” feature did not always update its narration after the user switched to a different slide.
- Some slides contained only a title even though the narration included substantial information that could have appeared as visible slide content.
- Long decks were difficult to navigate because the list view lacked page numbers, a section-based table of contents, and content-aware search.
- The purpose and behavior of some controls, including sharing and voting controls, were not clear to first-time users.
- Students could not find an obvious way to download the slides, and the Share button did not provide clear feedback about whether an action had occurred.
- Some subtitle slides were unnecessary and interrupted the flow of the deck when students reviewed it as study material.

## Prior Art & Originality

See instructions. Delete this line and replace with a short statement of what your team checked (the project's Future Work and Open Questions, its roadmap, and its open issues and pull requests) and which parts of your proposal are original — new work not already specified, scheduled, or proposed by someone else.

## Stakeholders

See instructions. Delete this line and replace with the name(s) of the stakeholder(s) you interviewed and lists showing their goals/needs, and problems/frustrations. Note which type of user each stakeholder represents. You may use pseudonyms or partial names to maintain their privacy, but you must privately share their full names and contact information as part of your submission of this exercise

## Product Vision Statement

See instructions. Delete this line and place your Product Vision Statement here — one sentence describing the improvements and new features your team is proposing for The Slide Machine.

## User Requirements

Our proposal focuses on improving the post-lecture experience. Instructors can refine live-generated presentations using the full lecture transcript, while students can more easily navigate, search, and review the resulting decks.

### Instructor

- As an instructor, I want to generate a refined presentation from the full lecture transcript so that the slides reflect the lecture as a whole.
- As an instructor, I want the system to identify the main topics and distinguish them from minor details so that the refined slides emphasize the most important material.
- As an instructor, I want the system to group closely related concepts and present parallel concepts consistently so that the organization of the deck reflects the structure of my lecture.
- As an instructor, I want the system to reduce repeated information so that the refined presentation is concise and does not unnecessarily repeat the same points.
- As an instructor, I want the system to preserve important explanations and examples from my lecture so that the refined presentation still reflects how I taught the material.
- As an instructor, I want the refined slides to follow the order and progression of my lecture so that the presentation matches how I introduced and explained the material.
- As an instructor, I want the system to choose slide boundaries based on changes in meaning and topic so that related information is not split across slides at awkward points.
- As an instructor, I want the refined presentation to be created as a separate deck so that the original live-generated presentation is preserved.
- As an instructor, I want to compare the original and refined presentations so that I can understand what the system changed.
- As an instructor, I want to regenerate the refined presentation so that I can request a different result if I am not satisfied with the first version.
- As an instructor, I want to correct the transcript before generating the refined presentation so that transcription errors do not become errors in the new slides.
- As an instructor, I want the system to notify me when refinement fails and preserve the original deck so that I know what happened without losing my existing presentation.
- As an instructor, I want to select an individual slide and give the AI a specific editing instruction while allowing it to use the full lecture transcript as context so that the revised slide remains consistent with the lecture.
- As an instructor, I want to select multiple slides and apply one AI editing instruction to all of them while allowing the system to use the full lecture transcript as context so that related slides are revised consistently.

### Student

- As a student, I want to view the refined presentation after the lecture so that I can review what the instructor actually covered.
- As a student, I want the refined presentation to include the main ideas from the lecture so that I can use it as a reliable study resource.
- As a student, I want related concepts to appear together so that I can understand how the ideas are connected.
- As a student, I want important explanations and examples from the lecture to be preserved so that the slides remain understandable outside the live lecture.
- As a student, I want repeated information to be reduced so that I can review the presentation efficiently.
- As a student, I want the slides to follow the order of the lecture so that I can connect them to what I remember from class.
- As a student, I want the deck to be divided into clearly labeled sections so that I can understand where one topic ends and another begins.
- As a student, I want to view a table of contents organized by lecture section and jump directly to a selected section so that I can navigate a long deck without repeatedly scrolling through it.
- As a student, I want to describe a concept in my own words and be directed to the relevant slide so that I can find information without remembering the exact wording used in the deck.
- As a student, I want search results to include the matching slide number and a short relevant excerpt so that I can identify the most useful result before opening it.
- As a student, I want the search system to use both the visible slide content and the lecture transcript so that I can find material that the instructor discussed even when it was not written directly on a slide.
- As a student, I want to return easily to the table of contents or my search results after reviewing a slide so that I can continue exploring the deck without losing my place.

## Activity Diagrams

### Student: Content-Aware Slide Search

**User story:** As a student, I want to describe a concept in my own words and be directed to the relevant slide so that I can find information without remembering the exact wording used in the deck.

![Content-aware slide search activity diagram](images/activity-diagrams/content-aware-slide-search.png)

### Student: Section-Based Navigation

**User story:** As a student, I want to view a table of contents organized by lecture section and jump directly to a selected section so that I can navigate a long slide deck without repeatedly scrolling through it.

![Section-based navigation activity diagram](images/activity-diagrams/section-based-navigation.png)

## Wireframes

See instructions. Delete this line and place your wireframe diagrams here, covering every new screen and every existing screen your proposal changes, for every type of user.

## Clickable Prototype

See instructions. Delete this line and place a publicly-accessible link to your clickable prototype here.

## Stakeholder Demo

See instructions. Delete this line and place a link to the deck The Slide Machine generated during your presentation here, after you have presented.

## Exit Ticket

See instructions. Delete this line and place a link to the exit-ticket quiz you generated from your demo deck and distributed to the class, along with a short note on what — if anything — you had to correct in the generated questions before publishing.
