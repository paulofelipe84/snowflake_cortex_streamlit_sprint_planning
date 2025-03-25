# Agile Sprint Planning with Cortex

This repository contains a Streamlit application designed to facilitate Agile sprint planning, integrating seamlessly with Snowflake's Cortex AI. The application allows users to convert requirements into Agile epics, break epics into user stories, and further split stories into actionable tasks, streamlining Agile workflow automation.

---

## Overview

The Agile Sprint Planning application provides an intuitive, interactive interface for Agile teams, leveraging AI-generated content to enhance productivity and maintain consistency across planning sessions.

### Key Features

- **AI-Assisted Agile Planning:** Utilises Snowflake Cortex AI (`llama3-8b` model) to generate epics, user stories, and task breakdowns automatically.
- **Dynamic Interaction:** Cards representing requirements, epics, stories, and tasks can be edited, expanded, or deleted interactively.
- **Visual Organisation:** A structured column layout clearly separates the Agile phases (Requirements → Epics → User Stories → Tasks).
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

- Python 3.8 or higher
- Streamlit (`pip install streamlit`)
- Snowflake account with Cortex enabled

### Running the Application

1. Clone this repository:

```bash
git clone https://github.com/your-username/agile-sprint-cortex.git
cd agile-sprint-cortex
```

2. Install required dependencies:

```bash
pip install -r requirements.txt
```

3. Configure your Snowflake connection within Streamlit to activate the Snowpark session.

4. Run the Streamlit app:

```bash
streamlit run your_script.py
```

---

## How to Use

1. **Add Requirements:** Start by clicking ➕ in the Requirements column to input business requirements.

2. **Generate Epics:** Convert requirements into detailed Agile epics by clicking the AI-generated action button on each requirement card.

3. **Generate User Stories:** Select the epic and automatically create relevant user stories with clear descriptions and acceptance criteria.

4. **Breakdown Tasks:** Break each user story into clearly defined, actionable tasks automatically.

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

