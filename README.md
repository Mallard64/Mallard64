### Hi, I'm Felix

Student building software and studying how to evaluate AI systems. I like projects with real users or real measurements behind them.

**AI evaluation**

- **[Inspec](https://github.com/Mallard64/inspec)**: Visual QA for assembled kits, with the packing list as the spec. An LLM compiles the list into explicit checks, SAM segments every part, and plain code counts and measures the masks. Checks that fail on known-good kits get repaired automatically (60/60 good kits wrongly rejected before repair, 2/60 after). On held-out MVTec LOCO AD images it catches 137/137 wrong-part errors on Screw Bag vs 130/137 for the vision model alone. Built solo for the Meta Global AI Developer Hackathon.
- **[upshift](https://github.com/Mallard64/upshift)**: Moves a multi-step LLM app off a retiring model without silent regressions. It replays recorded test cases on the old and new models (3 runs each), swaps models one step at a time to find which step regressed, removes prompt lines one at a time to find the guilty line, then proposes a minimal fix for human review. On planted bugs it named the correct step every time it named one. Built at a hackathon with a teammate.
- **[tutor-grader-transfer](https://github.com/Mallard64/tutor-grader-transfer)**: Does a grader trained to rate math tutor responses still work on programming tutoring? Not zero-shot: macro-F1 drops to 0.210, below the 0.272 majority-class floor. I measured how many programming examples it takes to recover, and found that the answer depends on the model. A TF-IDF grader's math pretraining starts to hurt after about 32 examples; DeBERTa's keeps helping. DeBERTa, TF-IDF, and an LLM judge, with 5 seeds and bootstrap CIs.

**Projects**

- **[Companion Connect](https://github.com/Mallard64/Companion_Connect)**: AI companion and journaling app for loneliness and social anxiety. Shipped to the iOS App Store with a student team; 2,000+ users in 4 countries, peak 500+ daily. React, Capacitor, Supabase, OpenAI behind an edge-function proxy.
- **[OmniSTEM](https://github.com/Mallard64/stemduolingo)**: Duolingo-style AP Chemistry app. GPT-4o generates questions, which are validated with zod against the College Board course framework, with an eval harness for the generator. Next.js, TypeScript, Supabase.
- **[Robot Rush](https://github.com/Mallard64/robot-rush)**: Online multiplayer arena shooter in Unity. Mirror networking, Hathora dedicated servers, Firebase.
- **[Resonance](https://github.com/Mallard64/resonance)**: 1v1 fighting game with server-authoritative netcode (Photon Fusion 2 host mode) and a bot opponent.
- **[Hunt the Wumpus: AI Edition](https://github.com/Mallard64/Wumpus)**: The 1973 cave game, where hazards become LLM-generated trivia duels with validated structured output and an offline fallback.

**Stack:** Python, PyTorch, Hugging Face · TypeScript, React, Next.js · C#, Unity · Supabase, Postgres, Firebase

**Contact:** [LinkedIn](https://www.linkedin.com/in/fxdeng/)
