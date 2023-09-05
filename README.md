# Data Wrangling - U.S. Macroeconomic Data (From 1959-2009)

Notes:
1. Starting with a problem
    * Start with a problem or a question
    * Why do we care about this problem or question?
    * How does it relate to our business or our goals?
    * What will the answer enable me to do?
    * Is there certain timeframe we are looking at or a certain segment of our users/data?
2. Identifying the right data to use
    * Is there any documentation available explaining each variable? Is one data source enough or do I need to join data together, and if so, do I know what column(s) to join on?
    * If I am joining data together, make sure it represents the same thing - the same timeline or locations or users.
3. Determining the scope of my solution
    * What is the deliverable the viewer expects? A dashboard or machine learning model put into production or just a summary of my findings?
    * What questions will I need to have answered before I can consider the project to be "done"?
4. Cleaning and preparing the data
    * What timeframe I should look at?
    * Other filters to limit the view of the data to what is relevant
    * Any variables that will help me segment or group my data - what is relevant to my questions or problem?
    * Examples can include gender, age, and other demographic factors, location, customer or user type, technology type, etc.
    * Once I have my data it should be cleaned and prepared. Even the cleanest and most perfectly collected data often needs some preparation - creating new variables or aggregating data. And often after doing the next step is exploration. I might find more that needs to be cleaned.
    * Check for missing varables - decide if I can leave them as NULL or if I need to replace them
    * Check for incorrect data types. Are my dates actually formatted as dates? Are all my numeric values actually integers or floats?
    * Check for distributions of numeric variables. Are there outliers? Decide what to do with them.
    * Check my categorical variables - is there anything wrong? Any unexpected values?
    * Are there any variables I don't need? Drop them or create a version 2 of my data without those columns?
    * Do I need to create any new variables? For example, do I want to create bins for any numeric variables? Create any new calculated metrics based on existing columns?
5. Exploring the data
    * Before getting to the problem I'm trying to solve, familiarize yourself with the data. These are some common things to look at:
    * Check the distributions for any numeric variables. A histogram is a good way to visually do this.
    * Check the count, mean, median, standard deviation, minimum, maximum, and quartiles of my numeric variables.
    * Check the count of my categorical variables.
    * Compare the numeric values when grouping by categorical variables.
    * Check for correlations of my numeric variables - what's the numeric value or visualize with scatterplots.
6. Solving the problem
    * Now that I have clean data that I am familiar with, solve my initial problem or answer my initial question.
    * "If you agreed on a dashboard and/or your stakeholder is going to need updated data in the future, build a dashboard that is clean and easy for them to navigate. Use headings and labels to make it easy for a viewer to understand what they are looking at. Add filters so they can self-serve different views of the data. Add a link to a document that defines all of the variables in your dashboard."
7. Summary
    * One framework for the summary is the S.T.A.R. method. This is also good for talking about your projects in an interview:
    * Situation: What is the business problem I'm trying to solve or question I'm answering? Why is it important?
    * Task: What is the goal or intended outcome?
    * Actions: What steps did I take? This section might have more or less detail or technical explanations depending on my audience.
    * Results: What was the actual outcome? What are my insights? What are my recommendations? How can my audience use this information to improve the business?
    
Questions:
