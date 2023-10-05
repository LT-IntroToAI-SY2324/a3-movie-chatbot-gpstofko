# Assignment 3 - Writeup

Assignment 3 is all about creating this natural language query system.  In order to do so, you have to write a lot of functions to retrieve infomation.  You will also have to write a function to return answers from a pattern-action list.  There is a lot of work to accomplish in this assignment, but this portion is intended for you to write about what you accomplished.

## Reflection Questions
1. In your own words describe the `search_pa_list` function.
The search_pa_list function takes an input called src, and first compares it to each pattern in pa_list. If a match is found, the difference is run to a subsequent movie search function to match the info to a movie. It then returns the found movie info. If a match is found but no info can be reteived "No answers" is returned. If a movie is not found that matches then "I don't know" is returned.

2. What movie did you add to the `movies.py` file?  What year was it made? Any specific reason you added that movie?
I added the movie interstellar made in 2014 because its a movie I really adore as when I grow up I want to pursue a career with something to do with space.

3. What pattern / action did you add to the paList data structure?  Why do you think that is a useful pattern / action?
(str.split("_ movies"), title_by_year),
I added this pattern / action because some people may want quick answers and to not type out full sentences so this pattern/action not onl gives another possivle question to ask but improve the efficiency of the user.

4. What is chatbot would you create that would be like this?  Describe why you would create it and what it would do.
I would like to create a chatbot that could search a database of songs and find songs made by certain authors in certain years.

5. What was the most difficult portion of this assignment?
The most difficult portion of this assignment was the search_pa_list function as my understanding of python wasn't deep enough to make the correct if statement and access different parts of tuples.

6. Did you write a new assert for your pattern action?
I did. I wrote the assert:
assert sorted(
        search_pa_list(["2014", "movies"])
    ) == sorted(["interstellar"]), "failed search_pa_list test 4"


