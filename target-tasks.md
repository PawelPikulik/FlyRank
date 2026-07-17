# Three Target Tasks for FL-02 through FL-04

These are the tasks I will reuse and deepen across the next three phases. Each has a measurable success definition.

---

## Task 1: Debug and integrate third-party APIs (e.g., CoffeeDB.pro)

- **Why this task**: It is the technical backbone of my proof. If I cannot reliably connect a live API to a conversational product, my claim collapses.
- **FL-02–04 focus**: Build the live API integration layer for Achilles; handle auth, rate limits, error states, and response parsing.
- **Done well means**:
  - API calls return valid data >95% of the time in production-like tests.
  - Error handling is explicit: timeouts, 4xx/5xx, and malformed responses all have defined fallback behavior.
  - I can explain the integration architecture to a Head of AI in two sentences without looking at code.
- **Measurable check**: Run 50 consecutive API calls and log failures. If >3 fail, fix the integration before moving to FL-03.

---

## Task 2: Pressure-test portfolio copy and design decisions against claim + audience + action

- **Why this task**: It is the strategic backbone of my proof. Every page, headline, and CTA must serve the Head of AI and lead to action. Vague copy kills the portfolio.
- **FL-02–04 focus**: Apply the pressure-test method to every deliverable: hero copy, case study structure, UI wireframes, and final build.
- **Done well means**:
  - Every headline names the audience's problem, not my skill.
  - Every page has one explicit CTA that bridges to the next step or Contact.
  - I can defend any line of copy against the question: "Does this serve the Head of AI specifically?"
- **Measurable check**: Before shipping any page, run the pressure-test prompt. If Claude finds more than one generic line, rewrite before building.

---

## Task 3: Iterate on AI agent prompts based on real user test conversations

- **Why this task**: It proves the "usable interface" part of my claim. A beautiful UI that returns wrong answers is decoration, not proof.
- **FL-02–04 focus**: Design, test, and refine the conversation prompts for Achilles. Test with real coffee questions, collect failure modes, and iterate.
- **Done well means**:
  - Achilles answers 10/10 common coffee questions correctly using live CoffeeDB.pro data.
  - Memory (preferences) persists across sessions and improves recommendations.
  - I can show a before/after of a prompt change that fixed a real failure.
- **Measurable check**: Run a test script with 10 representative queries. If >1 answer is wrong or uses stale data, iterate the prompt before FL-03.

---

## Why These Three

- **Task 1** is the *technical* proof (API → product).
- **Task 2** is the *strategic* proof (audience → action).
- **Task 3** is the * experiential* proof (conversation → memory).

Together they cover the full stack of my claim: "I ship domain-specific AI products from API to UI."
