# Project Overview
You are building a Reddit analytics platform, where users can get analytics of different sub reddits, where they can see top contents & see category of posts;

You will be using NextJS 14, shadcn, tailwing, Lucid icon

# Core functionalities
1. See list of available sub reddits & add new sub reddits
    1. User can see list of available sub reddits that already created display in cards, common ones like "ollama", "openai"
    2. Users can clich on an add reddit buttonm which shoul open a modal for user to paste in reddit url and add
    3. After users adding a new reddit, a new card should be added
2. Subreddit page
    1. Clicking on each subreddit, should go to a reddit page
    2. With 2 tabs: "Top posts", "Themes"
3. Fetch reddit posts data in "Top posts"
    1. Under "Top posts" page, we want to display fetched reddit posts from past 24 hrs
    2. We will use snoowrap as library to fetch reddit data
    3. Each post including title, score, content, url, creted_utc, num_comments
    4. Display the reddits in a table component, sort based on num of score
4. Analyse reddit posts data in "Themes"
    1. For each postm we should send post date to OpenAi using structured output to categorise "Solution requests", "Pain & anger", "Advice requests", "Money talk";
        1. "Solution requests": Posts where people are seeking solutions for problems
        2. "Pain & anger": Post where people are expressing pains or anger
        3. "Advice requests": Posts where people are seeking advice
        4. "money talk": Posts where people are talking about spending money
    2. This process needs to be ran concurrently for posts, so it will be faster
    3. In "Themes" page, we should display each category as a card, with tile, description & num of counts
    4. Clicking on the card will open side panel to display all posts under this category
5. Ability to add new theme category
    1. Users should be able to add a new card
    2. After a new card is added, it should trigger the analysis again

# Doc
XXXXX

# Current file structure
XXXXX
