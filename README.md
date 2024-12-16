# DAEN-690-CAPSTONE-PROJECT
GMU Mason Student Services Center (MSSC) &amp; GMU Information Technology Services (ITS) — Generative AI Chatbot 6-month Pilot Setup

## GMU Mason Student Services Center (MSSC) Generative AI Chatbot — 6-Month Pilot

### Abstract 

This project established the groundwork for a six-month pilot of a Generative AI Chatbot aimed at enhancing student support services at the Mason Student Services Center (MSSC) at George Mason University (GMU). Results from the Spring 2024 project highlighted the need for a scalable solution to provide 24/7 support, addressing gaps in MSSC’s availability during off-hours and periods of high demand. In preparation for the pilot, key architectural updates were implemented, including integrating the advanced Claude 3.5 Sonnet language model, reindexing the MSSC knowledge base using Kendra to ensure updated and relevant responses, and refining prompt engineering to enhance the chatbot’s contextual understanding and accuracy. While automated testing tools were initially considered for evaluating response quality, they were deemed unsuitable for this project, leading to the development of a manual testing framework that assessed the chatbot’s accuracy, relevance, and sensitivity to user emotions. Testing also included handling ambiguous or misleading queries and ensuring adherence to privacy standards. At the conclusion of the project, the updated chatbot system, along with supporting documentation for maintenance and upgrades, will be handed over to MSSC and ITS for the implementation of the six-month pilot, paving the way for improved accessibility and efficiency in student services through advanced AI solutions.

### 6-Month pilot task 

Rebuild the Kendra RAG Intelligent Search Index

Rebuild the AWS OnABot Environment

Upgrade the LLM to Anthropic Claude 3.5 Sonnet

Update the Chatbot Interface with GMU Branding

Modify the Prompt Engineering prompt passed to the LLM

Perform Unit Testing to Evaluate the Quality of LLM Responses

Collaborate with MSSC and ITS to define the Test Plan for the 6-month Pilot

### Estimated Costs for the 6-Month Pilot

Average Monthly Cost: $989.43

6-Month Total Estimate: Up to $5,940
Cost Breakdown:

Amazon Kendra: Fixed cost of $27/day (~$810/month).
This accounts for a significant portion of the expenses, as AWS Kendra Intelligent Search incurs a minimum charge even when not in use.

Other Services: Variable costs based on usage, including:
Token processing for the LLM via AWS Bedrock,Search queries on Amazon Kendra and Backend services like AWS Lambda and Amazon S3.
The average daily cost was $34, highlighting the dominance of fixed costs while leaving room for variability based on usage and system activity.

### Challenges faced 

### Rebuilding the environment
⁠IAM ACCESS ISSUES - requires full administrative rights to deploy the cloud formation stack.
⁠Redesign of the June 2024 QnABot cloud formation stack.
Reorganization the content designer settings.
### Unit testing
A requirement of the project was to evaluate the quality of LLM responses.
The initial tool selected, RefChecker, was not designed to work in a QnAbot solution architecture.
Bedrock LLM model evaluation tool is intended to evaluate different LLM models and was unsuitable to evaluate the quality of the LLM responses.
⁠Team instead focused on refining the prompt engineering process and manually evaluating the responses to the questions.

### Summary 
Rebuilt the chatbot environment to establish a stable foundation for future updates.
Reindexed the MSSC knowledge base using Amazon Kendra to ensure comprehensive and up-to-date search capabilities.
Upgraded the language model to Anthropic Claude 3.5 Sonnet via Amazon Bedrock, improving the chatbot's overall performance.
Enhanced prompt engineering to improve clarity, relevance, and quality of responses, particularly in handling personal information queries.
Conducted manual testing to evaluate response accuracy, relevance, and context awareness, identifying key areas for further improvement.

### Future work
The MSSC Chatbot needs to be aligned and integrated with the university-wide vision for AI.

### Partner Organizations
Amazon Kendra Web Crawler v2
Crawl Depth: 3
- **Mason Student Services Center (MSSC)**: [https://mssc.gmu.edu/](https://mssc.gmu.edu/)
- **GMU Information Technology Services (ITS)**: [https://its.gmu.edu/](https://its.gmu.edu/)

### Data Sources

- MSSC Knowledge Base: [MSSC Knowledge Base](https://mason.my.site.com/SelfServiceHC/s/topiccatalog)

