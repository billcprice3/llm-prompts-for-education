Generating Interactive Learning Activities Using Local Offline Models
Bill Price, April 2026
Why This Matters
People creating Open Educational Resources (OER) often need simple interactive learning activities - flashcards, quizzes, practice exercises - to supplement their textbooks and course materials. Traditionally, this has meant either: learning to code from scratch (a significant barrier for most educators), using proprietary commercial platforms (Quizlet, H5P, etc.), or settling for static content without interactivity.
Large language models can generate these interactive activities through conversation, but the most capable models (Claude, ChatGPT, Gemini) are cloud-based services that raise questions about data privacy, vendor lock-in, and ongoing costs. This experiment explores an alternative: can open-source models running entirely on personal hardware produce usable interactive educational materials?
The Experiment: Multiplication Practice Tool
I tested whether a local open-source coding model could generate a simple interactive mathematics activity from a plain-English specification.
Specification given to the model:
Using HTML, CSS, and Javascript, generate an activity that will create a random 10-question multiplication test. All 10 questions will be presented at once, with 10 user-editable answer boxes. Each question will be in the form x * y, where x and y are both integers between 2 and 9. A “randomize” button at the bottom will re-shuffle all the problems. A “submit” button at the bottom will mark each line as correct or incorrect and show a final score out of 10.
Technical setup:
	•	Hardware: Framework 13 laptop (AMD Ryzen 7 7840U, 32GB RAM, running Nobara Linux)
	•	Model: Gemma 4 E4B (Google DeepMind’s “Effective 4 Billion” parameter model, released March 2026)
	•	Runtime: Ollama (open-source local LLM server)
	•	Interface: VSCodium IDE with Continue extension (open-source AI coding assistant)
Process:
After loading the Gemma 4 E4B model via Ollama, I submitted the specification through the Continue extension. The model processed the request locally for approximately 5 minutes, then generated a complete HTML file containing the interactive activity.
Result:
The activity rendered and functioned correctly on first try. Students can practice multiplication, randomize problems, submit answers, and receive immediate feedback - all in a self-contained HTML file that works in any modern browser without internet connection.
Minor quirk: The number input boxes include increment/decrement arrows (HTML5 number input default behavior), which is unnecessary but harmless. This could be refined with a follow-up prompt or manual CSS edit.
What This Demonstrates
Data sovereignty is achievable. The entire workflow - from specification to working activity - happened on my personal computer without sending any data to external servers. No company captured my vocabulary lists, student information, or pedagogical approaches. The HTML file I generated is mine to use, modify, share, or archive as I see fit.
Open-source models are approaching usability for educational content generation. While Gemma 4 E4B (4 billion effective parameters) successfully handled this task, it represents the lower end of what’s currently viable for code generation on consumer hardware. More complex activities would likely require larger models (the 26B or 31B Gemma 4 variants, or equivalent open-source alternatives), which demand more RAM and processing power but remain runnable on desktop computers with decent specifications.
The teacher’s workflow doesn’t need to change. The resulting HTML file works exactly like any other teaching material - you can email it to students, post it to Canvas, save it in a folder with other activities, or distribute it however you normally share resources. Students open it in a browser (Chrome, Firefox, Safari), complete the activity, and can screenshot or print results if submission is needed.
Current Limitations
Hardware requirements matter. While Gemma 4 E4B runs on a laptop with 32GB RAM, generating complex activities or using larger models for better output quality requires more capable hardware than many educators have access to.
Generation time is significant. Five minutes of processing for a simple 10-question activity is acceptable for one-time creation, but wouldn’t work for rapid iteration or bulk generation of many activities.
Output quality varies. Simple, well-defined tasks (like this multiplication practice) work reliably. More complex specifications (adaptive difficulty, sophisticated feedback, multimedia integration) might require larger models, multiple refinement prompts, or manual editing.
Submission/grading integration is manual. Unlike Learning Management System (LMS) plugins, these standalone HTML activities don’t automatically report scores back to Canvas or other platforms. Students would need to screenshot results, print to PDF, or use other workarounds if formal submission is required - though for low-stakes practice activities, this limitation often doesn’t matter.
Why Pursue This Anyway?
Avoiding platform lock-in. Commercial tools like Quizlet have demonstrated the risks of depending on proprietary platforms: features get paywalled, user experiences degrade, data gets monetized, and tools can disappear entirely. A self-contained HTML file can’t be enshittified - you control it permanently.
True OER requires open tooling. If we want genuinely open educational resources, we need the interactive components to be open too. An “open textbook” that requires proprietary platforms for its practice activities isn’t truly open.
Skills transfer and customization. Once you have the HTML file, you can modify it yourself (if you know some coding), ask another AI to modify it, or hire someone to customize it. The openness enables adaptation that proprietary platforms deliberately prevent.
This approach aligns with the broader goals of the open web: decentralized, user-controlled, persistent, and resistant to corporate enclosure.
Looking Forward
The landscape of local AI capabilities is evolving rapidly. Gemma 4 was released just weeks ago (March 2026). Six months from now, more capable models will likely run on similar hardware, generation times will decrease, and output quality will improve.
For educators creating OER materials, the vision is clear: being able to say “I need a simple interactive activity to illustrate this concept” and generating it through conversation with a local tool, producing a self-contained HTML file you fully own and control, without depending on cloud services or commercial platforms.
We’re not quite there yet for all use cases, but we’re getting closer. The tools are open-source, the models are open-weights, and the infrastructure for truly sovereign educational content creation is emerging.
If you’re interested in exploring this workflow, the software stack I used is freely available:
	•	Ollama: ollama.com (local LLM runtime)
	•	VSCodium: vscodium.com (open-source VS Code build)
	•	Continue: continue.dev (AI coding assistant extension)
	•	Gemma 4: Available via Ollama (ollama pull gemma4:e4b)
The multiplication practice activity I generated is available as a proof-of-concept, though I’m not distributing it publicly since it’s just a simple demonstration rather than polished educational resource.

This experiment was conducted as part of ongoing exploration into AI-assisted materials creation for open educational resources. For related work on using cloud-based AI (Claude) for similar purposes, see my presentation “Rapid Interactive Materials Creation with Claude Artifacts”.