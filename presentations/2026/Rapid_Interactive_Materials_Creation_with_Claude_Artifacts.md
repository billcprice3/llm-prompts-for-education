# Rapid Interactive Materials Creation with Claude Artifacts

Bill Price, 17 April 2026

Presented as part of _[Language Instruction and Generative AI at Pitt: a Working Group's Report](https://www.polyglot.pitt.edu/events/language-instruction-and-generative-ai-pitt-working-groups-report)_

## What Is Claude, and What Are Artifacts?

Claude is an AI assistant developed by Anthropic, available to University of Pittsburgh faculty and students through Pitt's institutional subscription at [claude.ai](https://claude.ai/). Beyond generating text, Claude can produce self-contained, interactive web applications called "Artifacts" which are fully functional HTML/JavaScript tools that run directly in the browser, require no installation, and can be shared via link with anyone who has a Pitt account.

For language instructors, this means that a vocabulary quiz, a flashcard deck, a listening activity, or a reading exercise with interactive components can go from an idea to a published, shareable activity in a single conversation, without writing any code yourself.

***

## A Real Example: Vocabulary Practice for Linguistics 0010

I was recently preparing students in my Ling 0010 - ESL Reading and Vocabulary course for an upcoming assessment covering 30 target words. I needed something students could use to practice independently, but I wanted to avoid the "freemium" commercial tools like Quizlet. (I've learned the hard way to avoid lock-in on platforms that might unpredictably yank features or degrade the user experience.)

I opened Claude, gave it the list of target words and some context about the course and assessment format, and asked for a list of possible interactive activity ideas. 

After a brief back-and-forth, Claude produced a cloze (fill-in-the-blank) exercise activity. Each item presents a sentence with a gap and four multiple-choice options. Selecting the correct answer lights it up green and advances to the next item; selecting an incorrect answer marks it red and allows the student to keep trying. 

The format of the activity was simple enough. But Claude not only handled programming the interface, but also drafting all the sentences and content, albeit based on the 30 target words I had provided it. This could have taken multiple hours to do by hand, but Claude drafted a workable version of an item bank within a minute.

Claude made a few tweaks and refinements to the activity based on my feedback, and soon, I was happy with the result.

Once the cloze exercize Artifact was built, I published it with a shareable link set to "Anyone in your organization," then posted that link on Canvas as an external resource. Students click through, log in with their Pitt credentials, and the activity opens in their browser. 

The whole process, from my first exploratory prompt to Canvas link, took under an hour.

**Limitation worth keeping in mind:** Claude-hosted Artifacts don't report scores back to Canvas or any LMS. They're appropriate for low-stakes practice and self-study, not for graded assessments that require score recording or academic integrity controls. My only goal was to provide students with a studying tool, though, so that issue did not interfere with my purposes.

***

## A Walkthrough: Building a French Flashcard Tool

To illustrate the workflow more explicitly, here's a step-by-step account of building a simple French kitchen vocabulary flashcard tool; the kind of thing any language instructor could replicate in about 15 minutes.

**Step 1: Provide the vocabulary and a clear task.**  
I gave Claude a list of 20 French kitchen vocabulary words with English translations and grammatical gender, then asked for a flashcard studying Artifact, with the cards color-coded by gender, with features like shuffle and "mark as learned."

Here is the exact message I sent:

> Here are 20 French vocabulary words for a kitchen lesson:
>
> 1.  la cuisine — kitchen
> 2.  le four — oven
> 3.  le réfrigérateur — refrigerator
> 4.  le congélateur — freezer
> 5.  la cuisinière — stove/range
> 6.  le micro-ondes — microwave
> 7.  l'évier (m.) — sink
> 8.  le lave-vaisselle — dishwasher
> 9.  le robinet — faucet
> 10.  la casserole — saucepan
> 11.  la poêle — frying pan
> 12.  la marmite — stockpot
> 13.  le couteau — knife
> 14.  la cuillère — spoon
> 15.  la fourchette — fork
> 16.  le bol — bowl
> 17.  l'assiette (f.) — plate
> 18.  le verre — glass
> 19.  la planche à découper — cutting board
> 20.  le torchon — dish towel
> 
> Your task is to create a flashcard studying artifact. Color code the cards by masculine and feminine gender. Include some appropriate extra features like shuffle, mark as learned, etc.

![Artifact version 1](artifact_1.png)

**Step 2: Refine visually.**  
The first version used white card text on pastel backgrounds, which I found hard to read. I simply told Claude: _"Please make the card text black instead of white."_ It updated the Artifact immediately.

![Artifact version 2](artifact_2.png)

**Step 3: Add functionality.**  
I asked Claude to add keyboard shortcuts: _"Add keyboard shortcuts if possible. down arrow to flip; left and right for previous and next; up arrow for mark learned."_ Claude implemented all of these in one step.

![Artifact version 3](artifact_3.png)

**Step 4: Save and publish.**  
I used the "Save as Artifact" button to name and preserve the tool, then published it with organization-wide link sharing. The finished activity is available here (log in with your Pitt email address):  
[https://claude.ai/artifacts/latest/a0f8b6c4-ecc9-4988-b7df-f501ccfd6443](https://claude.ai/artifacts/latest/a0f8b6c4-ecc9-4988-b7df-f501ccfd6443)

The key point: no HTML was written, no JavaScript was debugged. The conversation _was_ the development process.

![Artifact as published in web browser](artifact_4.png)

***

## The Bigger Picture

The cloze exercise and the flashcard tool are just examples of a much broader point. The actual takeaway is that Claude Artifacts give instructors a fast path to custom interactive materials that fit their exact pedagogical context, whatever that context happens to be. Just describe what you want, refine through conversation, publish, and share with students.

The trade-off is transparency: instructors should verify content accuracy before deployment, and students should ideally understand they're using practice materials whose creation was accelerated with AI assistance. 

But for low-stakes supplementary practice- filling in curricular gaps, providing extra ways to engage with materials, making studying more engaging- this workflow is fast, flexible, and genuinely useful.
