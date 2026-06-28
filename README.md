# Interview Prep AI Agent

Interview Prep AI Agent is a learning-based AI agent project that I am currently developing while exploring how AI agents work in real-world applications.

The main purpose of this project is to understand how to build multi-agent workflows using CrewAI. I am also using Serper API to allow the agents to perform web-based research, such as company research, interviewer research, and role-specific interview preparation.

This project is not a finished product yet. It is part of my learning journey as I practice building AI agents, connecting external APIs, designing agent workflows, and understanding how different agents can work together to complete a task.

## Project Purpose

I started this project to learn how AI agents can be used for interview preparation.

Instead of building a simple chatbot, I wanted to understand how multiple agents can work together with different responsibilities. For example, one agent can research a company, another agent can generate interview questions, and another agent can provide feedback on user answers.

The goal is to learn by developing the project step by step.

## What I Am Learning

Through this project, I am learning:

- How to create AI agents using CrewAI
- How to assign roles, goals, and tasks to different agents
- How to use Serper API for web search and research
- How to organize agents into a workflow
- How to generate interview questions based on company and role information
- How to provide feedback on user answers
- How to structure an AI agent project in Python
- How to manage API keys using environment variables

## Tech Stack

- Python
- CrewAI
- Serper API
- OpenAI API or another LLM provider
- python-dotenv for environment variables

## Current Project Idea

The idea behind this project is to create an AI-powered interview preparation assistant.

The system will take user inputs such as:

- Company name
- Job role
- Skills
- Experience level
- Interview type
- Optional interviewer details

Based on these inputs, the AI agents will perform research, generate interview questions, conduct a practice interview, and provide feedback.

## Planned Workflow

1. User provides interview preparation details.
2. CrewAI initializes different AI agents.
3. A research agent collects company-related information using Serper API.
4. An interviewer research agent looks for publicly available interviewer background information if provided.
5. A question generation agent creates interview questions based on the role and research.
6. The user answers the questions.
7. A feedback agent reviews the answers and gives improvement suggestions.
8. The user can improve the answers through an iterative feedback process.

## AI Agents

### Company Research Agent

This agent is responsible for researching the company, including its products, services, culture, recent news, and business focus.

### Interviewer Research Agent

This agent is planned to research publicly available interviewer information, such as professional background and areas of expertise.

### Question Generator Agent

This agent generates role-specific technical and behavioral interview questions.

### Interview Coach Agent

This agent simulates a practice interview by asking questions in a structured way.

### Feedback Agent

This agent reviews user answers and gives feedback on clarity, structure, technical accuracy, and confidence.

## APIs Used

### Serper API

Serper API is used to perform web searches. It helps the agents collect real-time information about companies, job roles, interview topics, and related research.

### LLM API

An LLM API is used to generate responses, questions, summaries, and feedback.

## Environment Variables

Create a `.env` file in the root folder and add your API keys:

```env
SERPER_API_KEY=your_serper_api_key_here
OPENAI_API_KEY=your_openai_api_key_here
```

Do not commit your `.env` file to GitHub.

## Installation

Clone the repository:

```bash
git clone https://github.com/Shankar1371/Crewai_interviewagent.git
```

Move into the project folder:

```bash
cd Crewai_interviewagent
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment:

For Windows:

```bash
venv\Scripts\activate
```

For macOS/Linux:

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the Project

```bash
python main.py
```

## Planned Project Structure

```text
Crewai_interviewagent/
|
├── agents/
│   ├── research_agent.py
│   ├── interviewer_agent.py
│   ├── question_agent.py
│   ├── coach_agent.py
│   └── feedback_agent.py
|
├── tasks/
│   ├── research_tasks.py
│   ├── interview_tasks.py
│   └── feedback_tasks.py
|
├── tools/
│   └── serper_tool.py
|
├── main.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## Current Status

This project is currently in the learning and development stage.

I am not presenting this as a completed product. I am using this project to practice AI agent development and understand how tools like CrewAI and Serper API can be combined to create useful workflows.

Current progress:

- Designed the basic interview preparation workflow
- Planned multiple AI agent responsibilities
- Started working with CrewAI
- Integrated or planning to integrate Serper API for research
- Working on agent task execution and response generation

## Future Improvements

Planned improvements include:

- Better question generation
- Answer scoring system
- More detailed feedback
- Resume-based interview preparation
- Job description parsing
- PDF report generation
- Simple web interface
- Voice-based mock interview support
- Interview history tracking

## Learning Goal

The main goal of this project is to improve my understanding of AI agents by building a practical project.

This project helps me learn how to break a problem into multiple agent tasks, connect APIs, manage workflows, and develop a useful AI-based interview preparation assistant step by step.

## Author

Sankar Punati

## License

This project is for learning and portfolio purposes.
