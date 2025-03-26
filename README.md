# Agile Sprint Planning with Cortex

This repository contains a Streamlit application designed to facilitate Agile sprint planning. The application integrates seamlessly with Snowflake's Cortex AI and allows users to convert requirements into Agile epics, break epics into user stories, and further split stories into actionable tasks, streamlining Agile workflow automation.

---

## Overview

The Agile Sprint Planning application provides an intuitive, interactive interface for Agile teams. It leverages AI-generated content to enhance productivity and maintain consistency across planning sessions.

### Key Features

- **AI-Assisted Agile Planning:** uses Snowflake Cortex AI (`llama3-8b` model) to automatically generate epics, user stories, and task breakdowns.
- **Dynamic Interaction:** Cards representing requirements, epics, stories, and tasks can be edited, expanded, or deleted interactively.
- **Visual Organisation:** A structured column layout separates the Agile phases (Requirements → Epics → User Stories → Tasks).
- **Highlighting Mechanism:** Easily tracks the relationships between tasks, stories, epics, and original requirements through visual highlighting.
- **State Management:** Efficient use of Streamlit's session state for seamless and dynamic UI interactions.

---

## Technology Stack

- **Frontend:** Streamlit (Python)
- **Backend/AI:** Snowflake Cortex (using Snowpark)
- **AI Model:** Llama3-8b

---

## Installation & Setup

### Prerequisites

- Snowflake account with Cortex enabled

### Running the Application

1. Clone this repository:

```bash
git clone https://github.com/your-username/agile-sprint-cortex.git
cd agile-sprint-cortex
```

2. Create a new Streamlit App in your Snowflake account
3. Paste the contents of sprint_planner.py into the project
4. Run it

---

## How to Use

1. **Add Requirements:** Start by clicking ➕ in the Requirements column to input business requirements. Prefer using Markdown language.

2. **Generate Epics:** Convert requirements into detailed Agile epics by clicking the AI-generated action button on each requirement card.

3. **Generate User Stories:** Select the epic and automatically create relevant user stories with precise descriptions and acceptance criteria.

4. **Breakdown Tasks:** automatically break each user story into clearly defined, actionable tasks.

5. **Edit & Manage:** Edit, expand, or delete epics, stories, and tasks as needed. Visual highlighting helps maintain clarity and traceability.

---

## Customisation

- Modify the prompt templates in functions such as `generate_epic`, `generate_user_stories`, and `break_story_into_tasks` to adapt the AI outputs to your specific Agile practices.
- Update CSS styling within the Streamlit app to match your brand or preferences.

---

## Contributions

Contributions are welcome! Please open issues for feature requests or submit pull requests for improvements.

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

