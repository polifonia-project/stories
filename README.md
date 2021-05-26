# Polifonia Stories

This is a shared common space to share stories for the Polifonia project. A story is a template for collecting requirements.

A story is composed of:
- **Persona**
    - It is a research-based description of a typical user.
    - It contains attributes such as name, age, occupation (if the persona has more than one role, indicate which one is their primary role and which one(s) the secondary role(s)), and relevant characteristics of the person such as their knowledge and skills and their interests.
-  **Goal**
    - It is a short textual description of the goal(s) that the persona needs to be addressed in the story.
    - maximum number of characters: 1200
    - The goal(s) is(are) also represented by a short (maximum 5) list of keywords.
- **Scenario**
    - It is a story describing how the persona's task/need/problem is solved before, during and after interaction with the resource/software/service being developed.
    - maximum number of characters: 1200
- **Competency questions (CQs)**
    - Question(s) the persona needs the resource/software/service to answer for satisfying their task/need/problem.
-  **Resources (optional)**
    - List of resources (with references/links) where it is expected or known that the persona can find what she's looking for.

## How to create a story

There is one folder for each Persona, named with the name of the Persona and their primary occupation.

1. Check all existing Personas (there is one subfolder for each Persona in the "stories" folder), in order to see if there is already the Persona you need for your story. You will find a readme file in each folder, describing the Persona.
2. If you find a Persona that suits you, create a new file in the respective folder, named ``Name-of-the-persona``#``progressive-number``_``KeywordRepresentingTheMainGoal``.``md``, and fill the file with your story, following this [example](https://github.com/polifonia-project/stories/blob/main/Sethus:%20Music%20Theorist/Sethus%231_ConflictingTheoreticalInterpretations.md).
3. If not, create a new folder, named ``Name-of-the-persona: Primary Occupation``. If the persona has more than one role, use the primary role for naming the folder. Then, create a readme file (``readme.md``) describing the persona (see this [example]( https://github.com/polifonia-project/stories/blob/main/Sethus:%20Music%20Theorist/readme.md)), and then a file with your story as this [example](https://github.com/polifonia-project/stories/blob/main/Sethus:%20Music%20Theorist/Sethus%231_ConflictingTheoreticalInterpretations.md).
4. Besides providing information about the four components of the story, you should additionally fill in a table with this information:
- ID (``Name-of-the-persona``#``progressive-number``_``KeywordRepresentingTheMainGoal``)
- Persona (name of the persona)
- Keywords (representing their goals)
- WP (WPs involved in the story)
- Pilots (pilots involved in the story)
- Priority based on a “wow” scale, reflecting the impact that would be achieved by addressing the story, choosing from:
    - must have (i.e. it is something that is already supported in other systems, it is state of the art)
    - life improver (i.e. I would be able to make the same discovery/work in significant less time)
    - life changer (i.e. I would be able to make discoveries/works that now cannot be done or are extremely hard to do)
    - breakthrough (i.e. this would be a breakthrough in my field)
5. After completing your story, you should update the "List of personas" and/or the "List of stories" in this ``README.md`` file.
- If you created a new Persona: add to "List of personas" the name of the folder, and a link to the folder, following the examples. Then, add to "List of stories" the name of the story you created, and a link to the file.
- If you reused an existing Persona for your story: add to "List of stories" the name of the story you created, and a link to the file.

## List of personas

- (add personas here)
- [Mark: Computational Musicologist](https://github.com/polifonia-project/stories/tree/main/Mark:%20Computational%20Musicologist)
- [Ortenz: Music Historian](https://github.com/polifonia-project/stories/tree/main/Ortenz:%20Music%20Historian)
- [Patrizia:ethnoantropologist](https://github.com/polifonia-project/stories/tree/main/Patrizia:ethnoantrhropologist)
- [Keoma: Architect](https://github.com/polifonia-project/stories/tree/main/Keoma:%20Architect)
- [Sethus: Music Theorist](https://github.com/polifonia-project/stories/tree/main/Sethus:%20Music%20Theorist)
- [Carolina: Music Historian](https://github.com/polifonia-project/stories/blob/main/Carolina:%20Music%20Historian)
- [Anna: Hearing Impaired](https://github.com/polifonia-project/stories/tree/main/anna:hearing-impaired)
- [David: Music Historian](https://github.com/polifonia-project/stories/tree/main/David:Music-Historian)

## List of stories

- (add stories here)
- [Mark#1_folkMusic](https://github.com/polifonia-project/stories/blob/main/Mark:%20Computational%20Musicologist/Mark%23_1folkMusic.md)
- [Ortenz#MusicAndChildhood](https://github.com/polifonia-project/stories/blob/main/Ortenz:%20Music%20Historian/Ortenz%23MusicAndChildhood.md)
- [Patrizia#1_IdentificationOfIntangibleElements](https://github.com/polifonia-project/stories/blob/main/Patrizia:ethnoantrhropologist/Patrizia%231_IdentificationOfIntangibleElements.md)
- [Keoma#1_RestorationAndSoundPractices](https://github.com/polifonia-project/stories/blob/main/Keoma:%20Architect/Keoma%231_RestorationAndSoundPractices.md)
- [Sethus#1_ConflictingTheoreticalInterpretations](https://github.com/polifonia-project/stories/blob/main/Sethus:%20Music%20Theorist/Sethus%231_ConflictingTheoreticalInterpretations.md)
- [Sethus#1_CreateRelevantCorpus](https://github.com/polifonia-project/stories/blob/main/Sethus:%20Music%20Theorist/CreateRelevantCorpus.md)
- [Carolina#1_SourcesCrossAnalysis](https://github.com/polifonia-project/stories/blob/main/Carolina:%20Music%20Historian/Carolina%231_SourcesCrossAnalysis.md)
- [Anna#1_FeelingMusic](https://github.com/polifonia-project/stories/blob/main/anna:hearing-impaired/Anna%231_hearingMusic.md)
- [David#1_NonEliteMusic](https://github.com/polifonia-project/stories/blob/main/David:Music-Historian/David%231_musichistorian.md)


## Useful links

GitHub guides:
- Index https://guides.github.com/
- Markdown https://guides.github.com/features/mastering-markdown/
- Markdown cheatsheet: https://www.markdownguide.org/cheat-sheet/
