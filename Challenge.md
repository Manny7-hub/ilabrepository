The Granite 13 Billion chat V2 (granite-13b-chat-v2) model is the chat-focused variant initialized from the pre-trained Granite Base 13 Billion Base V2 (granite-13b-base-v2) model. granite-13b-base-v2 has been trained using over 2.5T tokens. IBM Generative AI Large Language Foundation Models are Enterprise-level English-language models trained with large a volume of data that has been subjected to intensive pre-processing and careful analysis.

granite-13b-chat-v2 is a chat-focused model that was tuned to improve its ability to perform Retrieval Augmented Generation (RAG) use cases. In version 2.1.0, IBM has applied a novel alignment technique for LLMs using large-scale targeted alignment for a generalist LLM. This alignment technique significantly improves base model performance by knowledge infusion during the initial phase of alignment, and improves instruction following performance via skills and style infusion in the subsequent phase of alignment.

To support the training of large enterprise-grade foundation models like Granite.13b, IBM curated a massive dataset of relevant unstructured language data from sources across academia, the internet, enterprise (e.g., financial, legal), and program code. In a rare move from a major provider of proprietary LLMs, IBM demonstrated its commitment to transparency and responsible AI by publishing descriptions of its training dataset online.

The Granite pre-training dataset was created as a proprietary alternative to commonly used open-source data compilations for LLM training, such as “The Pile” or “C4”. Some domains that are key for enterprise natural language processing are relatively under-represented in these compilations.

Additionally, these data compilations have been criticised for containing toxic, harmful, or pirated content. By curating its own pre-training data corpus, IBM takes significant steps towards addressing these and other issues.
The IBM curated pre-training dataset is continually growing and evolving, with additional data reviewed and considered to be added to the corpus at regular intervals. In addition to increasing the size and scope of pre-training data, new versions of these datasets are regularly generated and maintained to reflect enhanced filtering capabilities (e.g., de-duplication and hate and profanity detection) and improved tooling.

Granite 13b’s initial phase of pre-training involved IBM curating 48 TB of data before pre-processing and 2.07 TB after pre-processing. All datasets were filtered English-text and code unstructured data files. There are no pre-defined labels or targets. All non-text artifacts (e.g., images, HTML tags, etc.) were removed. Specifically, the first version of this base model, granite.13b.v1, was trained on 1 trillion tokens generated from 14 datasets. The individual datasets used in the training are described below.
1)	arXiv: Over 1.8 million scientific paper pre-prints posted to arXiv.
2)	Common Crawl: Open repository of web crawl data.
3)	DeepMind Mathematics: Mathematical question and answer pairs data.
4)	Free Law: Public-domain legal opinions from US federal and state courts.
5)	GitHub Clean: Code data from CodeParrot covering a variety of coding languages.
6)	Hacker News: News on computer science and entrepreneurship, taken between 2007-2018.
7)	OpenWeb Text: Open-source version of OpenAI’s Web Text corpus containing web pages through 2019.
8)	Project Gutenberg (PG-19): A repository of free e-books with focus on older works for which U.S. copyright has expired.
9)	Pubmed Central: Biomedical and life sciences papers.
10)	SEC Filings: 10-K/Q filings from the US Securities and Exchange Commission (SEC) for the years 1934-2022.
11)	Stack Exchange: Anonymized set of all user-contributed content on the Stack Exchange network, a popular collection of websites centered around user-contributed questions and answers.
12)	USPTO: US patents granted from 1975 to May 2023, excluding design patents.
13)	Webhose: Unstructured web content converted into machine-readable data feeds acquired by IBM.
14)	Wikimedia: Eight English Wikimedia projects (enwiki, enwikibooks, enwikinews, enwikiquote, enwikisource, enwikiversity, enwikivoyage, enwiktionary). containing extracted plain text from pages and articles.
The second version of the base model, granite.13b.v2, continued pre-training of the granite.13b.v1 model on an additional 1.5T newly-curated tokens for a total of 2.5T tokens seen during pre-training. The datasets used in this second tranche of training tokens were a mixture of the same 14 datasets from granite.13b.v1 (with additional snapshots added from the Common Crawl) along with 6 new datasets described below; all new snapshots and datasets were processed according to the same procedure described in III.
15)	Earnings Call Transcripts: Transcripts from the quarterly earnings calls that companies hold with investors. The dataset reports a collection of earnings call transcripts, the related stock prices, and the sector index.
16)	EDGAR Filings: Annual reports from all the publicly traded companies in the US spanning a period of more than 25 years.
17)	FDIC: The data is from the annual submissions of the FDIC.
18)	Finance Text Books: A corpus from UMN’s Open Textbook Library, including a dump of all textbooks tagged as finance.
19)	Financial Research Papers: Publicly available financial research paper corpus.
20)	IBM Documentation: IBM redbooks and product documents.

The training of IBM Granite 13b is particularly relevant to business for several key reasons, as outlined in the IBM research paper:
1. Enhanced Accuracy and Reliability

    Large and Diverse Dataset: The Granite 13b model is trained on a vast and diverse dataset comprising 2.5 trillion tokens. This extensive training data includes a wide range of documents, ensuring that the model can provide accurate and contextually relevant responses. This accuracy is crucial for business applications such as customer service, data analysis, and automated reporting.
2. Customizability and Adaptability

    Supervised Fine-tuning: The Granite 13b model includes a variant, granite.13b.instruct, which has undergone supervised fine-tuning to enhance its instruction-following capabilities. This allows businesses to tailor the model to specific tasks and use cases, improving its effectiveness for enterprise applications.
    Alignment Methods: The granite.13b.chat variant benefits from novel alignment methods that improve the quality of generation and mitigate potential harms. This makes it suitable for applications requiring high-quality conversational AI, such as virtual assistants and chatbots.
3. Efficiency and Scalability
    Advanced Training Infrastructure: IBM utilizes its Vela AI supercomputer for training the Granite models. This high-performance infrastructure ensures that the models are trained efficiently and can handle the large-scale data processing needs of enterprises.
    Optimization Techniques: The use of advanced algorithms and optimization techniques, such as MultiQuery-Attention and FlashAttention, ensures that the models operate efficiently, reducing latency and improving performance in real-time applications.
4. Data Governance and Compliance

    Rigorous Data Governance: IBM employs a comprehensive data governance framework during the training process. This includes rigorous pre-processing steps like text extraction, de-duplication, language identification, and document quality annotation. Such measures ensure the integrity and quality of the data used for training, which is essential for maintaining compliance with legal and regulatory standards.
    Ethical AI Practices: The training process also involves mitigating socio-technical harms and ensuring that the model's outputs adhere to ethical guidelines. This focus on ethical AI makes Granite 13b a trustworthy solution for businesses concerned about the ethical implications of AI deployment.
5. Practical Business Applications

    Customer Service and Support: Granite 13b can be integrated into customer service platforms to provide accurate and timely responses to customer queries, improving customer satisfaction and operational efficiency.
    Content Generation and Analysis: The model's ability to generate coherent and contextually relevant text makes it valuable for content creation, summarization, and analysis tasks, supporting marketing, and communication efforts.
    Decision Support Systems: By leveraging its extensive training data and fine-tuned capabilities, Granite 13b can be used in decision support systems to provide insights and recommendations, enhancing business decision-making processes.

The training and capabilities of IBM Granite 13b make it a powerful tool for enhancing various business operations. Its combination of accuracy, customizability, efficiency, and compliance with ethical standards ensures that it can effectively support a wide range of enterprise applications, from customer service to data analysis and decision support. For more detailed information, refer to the IBM Research Paper on Granite Foundation Models.

Using IBM Watson Machine Learning, you can deploy machine learning models, scripts, and functions, and prompt templates for generative AI models. After you create deployments, you can test and manage them, and prepare your assets to deploy into pre-production and production environments to generate predictions and insights.

You can deploy and manage your assets in the following ways:

    Use a no-code approach: You can use a no-code approach to deploy and manage assets in a deployment space. 

    Use a custom-code approach You can use a custom-code approach to deploy and manage assets programmatically by using:

        Python client

        Watson Machine Learning API

        watsonx.ai API

Summary of Retrieval Augmented Generation (RAG) in IBM watsonx
Concept Overview:
Retrieval Augmented Generation (RAG) combines information retrieval with generative models to produce factually accurate outputs grounded in a knowledge base. This technique enhances the accuracy of generated content by incorporating relevant information retrieved from a predefined knowledge base.
Steps for Implementing RAG:

    Search Knowledge Base:
        Search your knowledge base for content related to the user's question.
        Knowledge bases can include wikis, GitHub files, product documentation, databases, etc.

    Augment Prompt with Context:
        Add relevant search results to your prompt as context.
        Include instructions like “Answer the following question using only information from the following passages.”

    Generate Output:
        Send the combined prompt text to the foundation model.
        The model uses the provided context to generate a factual and contextually accurate answer.

Components of RAG:

    Knowledge Base: Any collection of informational artifacts that can be queried (e.g., internal wikis, documentation, databases).
    Retriever: Tools that return relevant content from the knowledge base. This can include search tools like IBM Watson Discovery or vector databases that use semantic search.
    Generator: Any model in watsonx.ai that processes the prompt and generates the response based on the provided context.
For more details, visit the IBM Developer page on RAG.

You can connect watsonx.ai to watsonx.data programatically using a database connector.

To govern an AI model in IBM watsonx, such as Granite13b, follow these steps:
Getting Started

    Log in to IBM watsonx: Ensure you have an IBM watsonx account. If you don't have one, sign up for a free trial on the watsonx platform.
    Open Your Sandbox Project: This project is automatically created for you when you sign up.

Basic Governance Workflow

    Create and Associate Service Instance: If necessary, create the service instance that provides the governance tool you want to use and associate it with your project.
    Choose a Tool to Govern AI: Select from various tools provided in the tutorials to evaluate and track AI models.

Tutorials for Governing AI
Each tutorial includes a description of the tool, a video, instructions, and additional learning resources:

    Evaluate and Track a Prompt Template:
        Description: Evaluate a prompt template to measure the performance of a foundation model and track the prompt template through its lifecycle.
        Expertise: Beginner, No code
        Tool: Use the evaluation tool to track the prompt template.

    Evaluate a Machine Learning Model:
        Description: Deploy a model, configure monitors for the deployed model, and evaluate the model.
        Expertise: Intermediate, Low code
        Tool: Run a notebook to configure the models and use Watson OpenScale to evaluate.

Documentation and Resources

    Visit the watsonx Documentation: Find comprehensive documentation and tutorials.
    Quick Start Tutorials: Access more tutorials in the watsonx documentation.
    Videos: Watch videos showing many common tasks in watsonx.

Additional Learning

    Overview of watsonx: Understand the platform and its capabilities.
    watsonx Use Cases: Learn about various use cases for watsonx.
    Governing Assets with watsonx.governance: Discover how to govern AI assets effectively.
    Evaluating AI Models: Learn how to evaluate AI models using the tools provided.

Samples and Resources

    Resource Hub: Access sample datasets, projects, models, prompts, and notebooks to gain hands-on experience.
    Notebooks: Add notebooks to your project to start analyzing data and building models.
    Projects: Import projects that contain notebooks, datasets, prompts, and other assets.
    Datasets: Add datasets to your project to refine, analyze, and build models.
    Prompts: Use prompts in the Prompt Lab to interact with foundation models.
    Foundation Models: Use foundation models in the Prompt Lab for various tasks.

For more detailed information, refer to the IBM watsonx AI Governance Documentation.

To govern Granite 13b effectively, use key evaluation metrics that are appropriate to the use case.  metrics include:
Ethical Metrics

    Bias and Fairness: Ensure unbiased predictions and fair outcomes across demographic groups.
    Transparency and Explainability: Make the model's decision-making process understandable and publish transparency reports.
    Accountability: Track incidents and ensure decisions can be audited.

Operational Metrics

    Performance and Accuracy: Measure prediction accuracy and response time.
    Robustness and Reliability: Conduct stress tests and track failure rates.
    Scalability: Monitor resource utilization and assess scalability.

Security Metrics

    Data Security: Implement data encryption and access controls.
    Threat Detection and Response: Conduct vulnerability assessments and evaluate incident response plans.

User Impact Metrics

    User Satisfaction: Collect user feedback and monitor engagement.
    Compliance and Legal Adherence: Ensure regulatory compliance and conduct legal audits.

Environmental and Social Impact Metrics

    Sustainability: Monitor and reduce energy consumption and carbon footprint.
    Social Impact: Evaluate positive contributions and mitigate negative social impacts.

Implementation

    Dashboard and Reporting: Use a dashboard for real-time monitoring and generate reports.
    Periodic Reviews: Conduct regular reviews to ensure continuous improvement.
    Stakeholder Engagement: Involve stakeholders to refine governance practices.

These metrics will ensure Granite 13b operates ethically, efficiently, and in alignment with organizational and societal values.

The context window length is 8192 bytes.  Which can support approximate 5 turns in a conversation.

You can develop generative AI solutions using multi-shot prompting with foundation models such as Granite 13b in IBM watsonx.ai. You can generate prompts for different AI use cases such as generate, classify, summarize, or extract content from your input text. Choose from IBM models or open source models from Hugging Face. You can use mult-shot prompts with multiple seeded examples to tune foundation models to customize your prompt output or optimize inferencing performance.

IBM watsonx.ai provides a studio of integrated tools for working with generative AI capabilities that are powered by foundation models and for building machine learning models.  You need an IBM Cloud API Key to connect to the application. 
Connecting the watsonx.ai application

The admin must connect the application using the token before you can use the skill. If you're an admin user, follow these steps to connect the application:

    On the Orchestrate chat page, click the Add skills from the catalog button.
    Select the watsonx.ai(experimental) app.
    On the top right corner of the page, click the Connect app button.
    Enter the Bearer Token you retrieved from the IBM Cloud service.
    Click Connect app to proceed.

Using watsonx.ai skills
You can add watsonx.ai skills to your skill set to use it. For a list of available skills using watsonx.ai, see List of prebuilt apps, skills and skill flows.

To add the skill to your skill set:
    On the Orchestrate chat page, click the Add skills from the catalog button.
    Select the watsonx.ai(experimental) app.
    Select the skills that you want to use and click Add skill.
    Return to the chat to see the skills you have selected and click them to start the skill.

IBM provides an IP indemnity (contractual protection) for its foundation models, enabling its clients to be more confident AI creators by using their data, which is the source of competitive advantage in generative AI. Clients can develop AI applications using their own data along with the client protections, accuracy and trust afforded by IBM foundation models.

"When it comes to today's AI innovation boom, the businesses that are positioned for success are the ones outfitted with AI technologies that demonstrate success at scale and have built-in guardrails and practices that enable their responsible use," said Dinesh Nirmal, Senior Vice President, Products, IBM Software. "Today's release of IBM's Granite model series and commitment to stand behind IBM-developed watsonx models is a testament to IBM's end-to-end model lifecycle management process in its watsonx AI and data platform that delivers businesses cutting-edge AI outfitted for their unique business needs."

For more than a century, IBM has worked to earn the trust of business and society by ushering powerful new technologies, including AI, into the world responsibly and with clear purpose. To date, the company has built and made available a range of open source tools and AI governance software to help ground the creation and use of this technology in principles of transparency, explainability, privacy, robustness and fairness.

As the names suggests, Granite is a 13 billion parameter model set.

To use Watson Pipelines for tuning Granite 13b, you can follow these steps:
1. Access the components in your pipeline: Make sure that you have access to all of the elements in the pipeline, including assets, projects, and spaces used in the pipeline.
2. Manage pipeline credentials: Generate an API key from your IBM Cloud Pak for Data user account to execute long-running operations in the pipeline without disruption.
3. Add assets to a pipeline: Collect the assets, such as data, notebooks, deployment jobs, or Data Refinery jobs, in the project containing the pipeline and use the asset browser to select project assets for the pipeline.
4. Manage resources by setting memory limits: Set your Cloud Pak for Data instance's memory size limit of Redis to avoid memory overconsumption.
5. Update default runtime type: Update the default runtime type for nodes by updating your ConfigMap.

By following these steps, you can use Watson Pipelines for tuning Granite 13b and automate a flow to improve the performance and efficiency of the model.

IBM watsonx.governance was built to help you direct, manage and monitor the artificial intelligence (AI) activities of your organization.

    Govern generative AI (gen AI) and machine learning (ML) models from any vendor including IBM watsonx.ai, Amazon Sagemaker and Bedrock, Google Vertex and Microsoft Azure.
    Evaluate and monitor for model health, accuracy, drift, bias and gen AI quality. 
    Access powerful governance, risk and compliance capabilities featuring workflows with approvals, customizable dashboards, risk scorecards and reports.
    Use factsheet capabilities to collect and document model metadata automatically across the AI model lifecycle.

Granite solutions can either be developed from scratch, using API calls in programming languages like, say, Python, or developed using the Watsonx.AI user intereface, which can generate Python code directly. Development is therefore agnostic to either cloud or on premise environment placement.

Granite models can be tested in a number of ways  and is agnostic to the location of any test environment. Testing can be done from withing the watsonx.ai UI, for example as in zero or multishot promting, or via test harnesses for Python etc.

IBM was one of the earliest champions of open source, backing influential communities like Linux, Apache, and Eclipse, pushing for open licenses, open governance, and open standards.

Our first notable interaction with open source software was when a number of IBM engineers began contributing to Linux (yes, the Linux on which Red Hat Enterprise Linux is built). In the late 1990s, IBM supported Linux with patent pledges, a $1 billion investment of technical and other resources, and helped to establish the Linux Foundation in 2000.

In 1999, we helped to create the Apache Software Foundation (ASF), contributing thousands of line of code and dedicated resources to support the Apache Web Server projects. As a founding member, we helped shape the license and governance, served in leadership roles, and contributed to numerous projects. Today, there are over 200 projects on ASF, and the scope has widened from the original HTTP server project to include web technologies, XML, web services, document processing, mobile, cloud, big data and analytics, serverless, and messaging. Clearly, we helped create a safe place to collaborate and innovate in the open.

We led the creation of the Eclipse Foundation in 2004. We seeded the Eclipse project with a significant code contribution, dedicated developers, and legal help in writing the licenses. Now, there are over 360 projects at Eclipse covering a broad spectrum of technology. We credit Eclipse’s success to its open governance, giving open source developers a neutral place to collaborate and innovate in the open.

In its infancy, IBM recognized the promise of open source and contributed thousands of lines of code, man hours, and money to ensure that foundations were set up in a way that supported open governance and standards. On a broad scale, IBM’s participation in these and well over a thousand other projects and communities set the tone for open source adoption among enterprises.

Both Granite Chat and Granite Instruct 13b support Coding Type, Repitition Penalty, Stopping Criteria, Maximum Tokens and Minimum Tokens as hyperparameters.

Granite-13b-chat-v2 is a chat-focused model that was tuned to improve its ability to perform Retrieval Augmented Generation (RAG) use cases. granite.13b.instruct.v2 is an instruction-tuned model that was Supervised Fine-Tuned (SFT) tuned using a combination of the Flan Collection, 15k samples from Dolly, Anthropic's human preference data about helpfulness and harmlessness, Instructv3, and internal synthetic datasets specifically designed for summarization and dialogue tasks (~700K samples).

Granite 13b was trained by IBM Research

IBM’s Granite model is one of the most transparent LLMs in the world

A new report from Stanford University’s Center for Research on Foundation Models showed that IBM’s model scored a perfect 100% in several categories designed to measure how open models really are.   In many of the categories tested by the FMTI, IBM’s Granite model scored a perfect 100%, far surpassing the averages for those categories. In the risk mitigations category, Granite was the clear leader. In the data category, the Granite model performed better than any other model, barring ServiceNow’s Starcoder, which is a code model, rather than a natural-language model. IBM’s Granite model also scored a perfect 100% in the compute, methods, and model basics categories. Overall, IBM’s Granite model scored 64%, with only three of the models surveyed performing better.

The Benchmark MEASURING MASSIVE MULTITASK LANGUAGE UNDERSTANDING was used to measure a text model's multitask accuracy. The test covers 57 tasks including elementary mathematics, US history, computer science, law, and more.

MT-Bench was the	benchmark consisting of 80 high-quality multi-turn questions. MT-bench is designed to test multi-turn conversation and instruction-following ability, covering common use cases and focusing on challenging questions to differentiate models.

