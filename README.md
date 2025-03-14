# Database-Query-Generator
# Commands to run the project:
### command to run the application:
#### npm init
### npm start

# Project Details:

## Situation(Objective)
The objective of project is to create an AI-powered application that allows users
to interact with user-interface and get the query in return 

## Behavior(Solution):

Based on this situition the app needs to decide which datasets to query, and
how to generate the right output. One way to do this is to store that data into an
SQL database, and use an LLM to convert the user query into an SQL query to
retrieve the relevant data, and show it to the user. Another way to do it is to use an
LLM to parse the user query to extract key attributes, and then construct one or
more SQL query algorithmically, and retrieve and combine the data, and show it to
the user. There can be other ways to do this, like using Generative AI(openai)

### Deciding the Correct approach:

Generative AI and Large Language Models (LLMs) represent two highly dynamic and captivating domains within the field of artificial intelligence. Generative AI is a comprehensive field encompassing a wide array of AI systems dedicated to producing fresh and innovative content, spanning text, images, music, and code. In contrast, LLMs constitute a specific category of generative AI models with a specialized focus on text-based data.

#### Generative AI and LLM-Definition:
Generative AI refers to the broader concept of artificial intelligence models that have the ability to generate new content. These models are designed to create text or other forms of media based on patterns and examples they have been trained on. They use sophisticated algorithms to understand context, grammar, and style in order to produce coherent and meaningful output.
On the other hand, LLMs specifically focus on language modelling. These models are trained on vast amounts of text data and learn the statistical properties of language. They excel at predicting what comes next in a given sequence of words or generating text based on a prompt.

The Role of Generative AI and LLM Generative AI models undergo extensive training on large datasets to assimilate the underlying patterns and relationships present within that data. Once trained, they have the capacity to generate novel content that aligns with the characteristics of the training data. For instance, a generative AI model trained on images of cats can be harnessed to create entirely new cat images that haven’t been witnessed before. LLMs, on the other hand, undergo rigorous training on vast volumes of text data, encompassing sources like books, articles, and code. After their training is complete, LLMs are primed for text-related tasks, including text generation, language translation, and content creation across various genres, and providing informative responses to queries.
#### Scope of Generative AI and LLM
The key difference between generative AI and LLM lies in their scope.  Generative AI: Generative AI encompasses various types of models that can generate content beyond just textual data, including images or even music. Generative AI opens up possibilities for creating diverse forms of content beyond just text.
LLM: LLMs excel at understanding language patterns for accurate predictions and textual generation. LLMs are specialized in understanding and generating human-like text based on patterns they have learned from training data.
The Verdict: Choosing the right approach
When choosing between generative AI and large language models (LLMs), consider the following factors:
Type of content: Generative AI can generate images, music, code, and other types of content beyond text. LLMs are best suited for text-based tasks like natural language understanding, text generation, language translation, and textual analysis.
 Data availability: Generative AI requires diverse datasets for different types of content. LLMs are designed to work specifically with text and are a good choice if you have extensive text data.
Task complexity: Generative AI is appropriate for complex, creative content generation or tasks that require diversity in outputs. LLMs are specialized for language understanding and text generation, providing accurate and coherent text-based responses.
 Model size and resources: Larger generative AI models require more computational resources and storage. LLMs may be more efficient for text-focused tasks due to their specialization in language understanding.
 Training data quality: High-quality, diverse training data is essential for generative AI to produce meaningful and creative outputs. LLMs require large, clean text corpora for effective language understanding and generation.
 Application domain: Generative AI is a good fit for creative fields like art, music, or content creation. LLMs are well-suited for applications in natural language processing, including chatbots, content summarization, and language translation.
 Development expertise: Developing and fine-tuning generative AI models can be challenging and require expertise in machine learning and domain-specific knowledge. LLMs, especially pre-trained models, are more accessible and user-friendly for text-based tasks, requiring less specialized expertise.
Ethical and privacy considerations: Consider ethical concerns regarding the use of AI models, particularly if generating content or answering sensitive questions. LLMs are often fine-tuned to adhere to specific ethical guidelines.

Thus We will be implementing one of the approach: Generative AI

### Schema(structure of data) of the tables:
There tables in the database, one containing company info, one containing
people info. 
Events and company data can be merged using ‘event_url’ column.
Company and people data can be merged using ‘homepage_base_url’ column.

Each event_url corresponds to a unique event, and each homepage_base_url can
be interpreted as a unique company.

## Impact:
This will reduce the manual task & and labour of creating the query as per the requirement.Here the layman will also be able to get query for the data using simple language.
