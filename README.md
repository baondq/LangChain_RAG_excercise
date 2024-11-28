# LangChain_RAG_excercise

My notebook is structured as sequence of blocks. The following is explanation of each block.
1. Generate Real Estate Listings
- Init LLM and query for generate information of 10 houses
- Generate house information
- Write the generated outputs to Listings.txt
- Convert the generated texts to list of Documents
2. Storing Listings in a Vector Database
- Split documents to chunks
- Embed chunked documents and store them to Chroma database
3. Building the User Preference Interface
- create chat history
- summarize chat and store the summary to memory
4. Searching Based on Preferences
- Iterate over each preference, find top 3 similar listings with the preference. Add 1 matching score to these 3 listings.
- Sort listings according to their scores and get 3 highest score listings
5. Personalizing Listing Descriptions
- Init LLM and prompt template
- Augment prompt with house information and chat summary
- Generate new descriptions
