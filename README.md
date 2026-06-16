# Agentic AI: Build Your First Agentic AI System

This is the repository for the LinkedIn Learning course `Agentic AI: Build Your First Agentic AI System`. The full course is available from [LinkedIn Learning][lil-course-url].

![Agentic AI: Build Your First Agentic AI System][lil-thumbnail-url]

## Course Description

Dive into agentic AI and master the skills you need to build scalable, real-world systems within an enterprise environment. In this course, industry expert Aishwarya Naresh Reganti shows you how to identify suitable business problems for agentic AI solutions, break down systems, iterate designs from baseline to advanced setups, and evaluate design trade-offs. Learn how to apply a comprehensive CCCD (Continuous Calibration Continuous Development) framework to safely increase AI autonomy while maintaining user trust. Tackle complex AI challenges as you gain insights on guardrails, governance, and security. This course is suited for engineers, product managers, enterprise leaders, and anyone eager to move beyond AI basics and implementation hurdles. Whether you're enhancing your existing skills or seeking to refine AI systems from concept to execution, this course delivers valuable knowledge for practical applications.

## Instructions

This repository has branches for each of the videos in the course. You can use the branch pop up menu in GitHub to switch to a specific branch and take a look at the course at that stage, or you can add `/tree/BRANCH_NAME` to the URL to go to the branch you want to access.

## Course Notebooks

This course uses two main Jupyter notebooks that you'll run on Google Colab:

### Chapter 3: V1 Action Autonomy (Router Agent)
**[Open action_autonomy.ipynb in Colab](https://colab.research.google.com/github/subinksankaran/agentic-ai-build-your-first-agentic-ai-system-4645038/blob/main/action_autonomy.ipynb)** - Use this notebook throughout Chapter 3. The notebook includes clear chapter break markers (🎬 End of Chapter) that show you where to stop for each video.

### Chapter 4: V2 Planning Autonomy (Planning Agent)
**[Open planning_autonomy.ipynb in Colab](https://colab.research.google.com/github/subinksankaran/agentic-ai-build-your-first-agentic-ai-system-4645038/blob/main/planning_autonomy.ipynb)** - Use this notebook throughout Chapter 4. The notebook includes clear chapter break markers (🎬 End of Chapter) that show you where to stop for each video.

## Running the Notebooks

All notebooks in this course are designed to run on **Google Colab** with no local setup required.

### Quick Start with Google Colab

1. **Download the course files**: Download this repository as a ZIP file from LinkedIn Learning

2. **Open the notebook in Colab**: Click on the notebook link above (e.g., "Open action_autonomy.ipynb in Colab") to launch it directly in Google Colab

3. **Upload the course ZIP file**:
   - In Colab, click the folder icon (📁) in the left sidebar to open the Files panel
   - Drag and drop the downloaded ZIP file (`agentic-ai-build-your-first-agentic-ai-system-4645038.zip`) into the Files panel
   - Wait for the upload to complete

4. **Set up your OpenAI API key**:
   - In Colab, click the key icon (🔑) in the left sidebar
   - Add a new secret named `OPENAI_API_KEY`
   - Paste your OpenAI API key as the value
   - Toggle the "Notebook access" switch to enable access

5. **Run the setup cell**: Execute the first cell in the notebook - it will automatically unzip the course files and set up the environment

6. **Continue with the notebook**: Execute remaining cells in order, stopping at chapter break markers as indicated in the videos

## Prerequisites

- **OpenAI API Key**: You'll need an OpenAI API key to run the notebooks. [Get one here](https://platform.openai.com/api-keys)
- **Basic Python Knowledge**: Familiarity with Python and Jupyter notebooks is helpful
- **Google Account**: Required for using Google Colab

## What You'll Build

### V1: Action Autonomy (Router Agent)
A customer support routing agent that:
- Classifies customer messages into appropriate departments
- Uses systematic evaluation to measure baseline performance
- Applies error analysis to discover improvement opportunities
- Implements targeted improvements and validates results

**Key Concepts:**
- Simple prompt engineering
- Systematic evaluation
- Continuous Calibration (CC): Analyzing failures to discover improvements
- Continuous Deployment (CD): Implementing and validating improvements

### V2: Planning Autonomy (Planning Agent)
A multi-step planning agent that:
- Routes messages using V1's proven routing (builds on V1!)
- Retrieves relevant procedures from a knowledge base using BM25
- Generates detailed, multi-step action plans
- Uses custom metrics to measure and improve retrieval and plan quality

**Key Concepts:**
- RAG (Retrieval Augmented Generation) with BM25
- Custom metrics design from observations
- LLM-as-Judge for plan evaluation
- Incremental building (V2 = V1 + new capabilities)

## Course Structure

The course follows a systematic pattern for both autonomy levels:

1. **Build**: Implement the baseline system
2. **Test**: Run evaluation to establish baseline metrics
3. **Calibrate (CC)**: Observe failures, analyze patterns, design metrics
4. **Deploy (CD)**: Make targeted improvements, re-evaluate, validate gains

This CC/CD pattern works for production systems and teaches you how to systematically improve any agentic AI system.

## Repository Structure

```
├── action_autonomy.ipynb          # Chapter 3: V1 Action Autonomy
├── planning_autonomy.ipynb        # Chapter 4: V2 Planning Autonomy
├── data/
│   ├── v1_test_cases.csv          # Test cases for V1 evaluation
│   ├── v2_test_cases.csv          # Test cases for V2 evaluation
│   └── sops/                      # Standard Operating Procedures (V2)
│       ├── sop_001.txt
│       ├── sop_002.txt
│       └── ...
└── assets/
    └── diagrams/                  # Architecture diagrams
        ├── autonomy_ladder.png
        ├── v1_architecture.png
        ├── v2_architecture.png
        └── ...
```

## Troubleshooting

### "ModuleNotFoundError" in Colab
- Run the first cell that installs packages: `!pip install -q openai pandas ...`
- Restart the runtime if needed: Runtime > Restart runtime

### "Invalid API Key"
- Verify your OpenAI API key is set correctly in Colab Secrets
- Check that "Notebook access" is enabled for the secret

### Phoenix UI not loading
- Use the Colab-compatible Phoenix setup (already configured in notebooks)
- The Phoenix UI may take 30-60 seconds to start

### Images not displaying
- Images are loaded from the `assets/diagrams` folder in the repository
- Ensure you're viewing the notebook from the correct branch

## Additional Resources

- [Arize Phoenix Documentation](https://docs.arize.com/phoenix)
- [OpenAI API Documentation](https://platform.openai.com/docs)
- [BM25 Algorithm Explanation](https://en.wikipedia.org/wiki/Okapi_BM25)

## Instructor

**Aishwarya Naresh Reganti**

[0]: # (Replace these placeholder URLs with actual course URLs)

[lil-course-url]: https://www.linkedin.com/learning/agentic-ai-build-your-first-agentic-ai-system
[lil-thumbnail-url]: https://media.licdn.com/dms/image/v2/D4D0DAQETSarROpRJLw/learning-public-crop_675_1200/B4DZvz7obMIQAY-/0/1769324055075?e=2147483647&v=beta&t=0Ba3fWz4aMqr4b-9nk2om4vpy2aS6a8hBMf3BSKBJzk
