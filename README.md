# Content Researcher and Writer - Multi-Agent Crew

This project is a Streamlit-based web application that leverages the **CrewAI** framework to generate high-quality blog articles on user-specified topics. It uses an AI-powered multi-agent system consisting of three agents: a **Content Planner**, a **Content Writer**, and an **Editor**. Each agent uses advanced language models (LLMs) from Together AI to perform their tasks, ensuring engaging, factually accurate, and well-structured content.

## Features

- **Topic-Based Content Generation**: Users can input any topic, and the system generates a comprehensive blog post.
- **Multi-Agent Workflow**:
  - **Planner**: Researches the topic, identifies trends, analyzes the audience, and creates a detailed content outline with SEO keywords.
  - **Writer**: Crafts a compelling blog post based on the planner's outline, incorporating SEO keywords and ensuring proper structure.
  - **Editor**: Proofreads and aligns the blog post with journalistic best practices and the brand's voice.
- **Customizable Settings**: Adjust the LLM temperature via a slider to control creativity vs. precision.
- **Output**: Generates a downloadable blog post in Markdown format.
- **Interactive UI**: Built with Streamlit for a user-friendly experience.

## Tech Stack

- **Framework**: CrewAI for agentic AI workflows.
- **Frontend**: Streamlit for the web interface.
- **LLMs** (via Together AI):
  - Meta AI's Llama-4-Scout-17B-16E-Instruct (Planner)
  - Qwen3-235B-A22B-fp8-tput (Writer)
  - Google's Gemma-2-27b-it (Editor)
- **Tools**: SerperDevTool for web search and research.
- **Environment**: Configured for Hugging Face Spaces with proper directory setup for CrewAI.

## Prerequisites

To run this project locally or deploy it, ensure the following:

- Python 3.8+
- Required Python packages (listed in `requirements.txt`)
- API keys for:
  - **Together AI** (for LLMs)
  - **Serper API** (for web search)
- Environment variables set for `TOGETHER_API_KEY` and `SERPER_API_KEY`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/a-pragatheeswaran/PublicResearchWriteCrewAIMultiAgent.git
   cd PublicResearchWriteCrewAIMultiAgent
