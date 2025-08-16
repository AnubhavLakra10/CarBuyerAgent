# AI Agent for Smart Product Buyers

 ## Overview

 This notebook talks about the **Smart Product Buyer AI Agent**, which was made as a **Proof of Concept (PoC)** to help people make smart choices when they buy things.  The current version is mostly for buying cars, but it is made to be **easily extendable** to work with other websites and even other types of products.  The project uses **LangGraph** and **LLM-based intelligence** to make the user experience interactive, efficient, and flexible.

 ## Full Explanation

 ### Reason
 Modern shoppers have a hard time finding their way through the huge number of products available online.  This agent makes it easier to search and make decisions by: - Knowing what users want and need.
 - Improving and using complicated filters on many platforms.  It only works with AutoTrader right now, but you can easily add other platforms by putting a new scraper in the `scrapers` folder.
 - Giving useful information and suggestions.

 ### Important Parts
 1. **Processing User Input**: Uses LLM-powered interactions to dynamically figure out what users want and need.
 2. **Filter Refinement**: Adjusts search filters to fit the parameters set by the user.
 3. **Web Scraping and Integration**: Connects to sites like AutoTrader to get and show relevant listings.
 4. **Summarisation and Insights**: Gives short summaries and insights into listings, such as how reliable the overall market is.

 ### The Structure of the Agent
 The agent follows a set process:
 - **User Need Assessment**: Gathers and summarises what users want.
 - **Filter Building**: Makes and uses search filters.
 - **Listing Retrieval**: Gathers information from connected platforms.
 - **Insight Delivery**: Gives more information and suggestions.

 ### Good things
 - **Efficiency**: Cuts down on the time it takes to look for and compare products.
 - **Clarity**: It turns complicated data into useful information.
 - **Flexibility**: Works with more than just cars.
 ---

 ## Setting Up the Code

 The steps below will help you set up the right environment and run the agent.

 ### Things You Need
 Make sure that Python and Jupyter Notebook are both installed on your computer.

 You can run the project on Google Colab or any local Jupyter Notebook, but for some reason scraping is very slow on Google Colab.
 We suggest that you run the project on your own Jupyter Notebook, ideally on macOS or Linux.  If you have Windows, the best way to get the best performance is to run it under WSL.

 Just run all the cells in the notebook to open the Gradio interface. Then, click the link to connect to the Gradio interface.

 If you want to run the project without the Gradio interface, you can set the USE_GRADIO variable to False.  This makes it easier to test and fix problems with the project.

 Set up the .env file with the API keys you need:
 - OPENAI_API_KEY (required)
 - LANGCHAIN_API_KEY (not needed if LangSmith isn't used)