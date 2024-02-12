# Foundation Model: Large Language Model For Christmas Movies Review

<center><p float="center">
  <img src="https://www.wfla.com/wp-content/uploads/sites/71/2019/12/CHRISTMAS-MOVIES-2.jpg?w=876&h=493&crop=1" width=650/>
</p></center>

## Problem Statement

### Business Context
- Christmas has come to represent different things to people over the years, and the movies here reflect that in kind. If you’re traditional and feeling nostalgic,you’ll be pleased to see reviews on some of popular Christmas movies such as The Holiday, Bad Santa, Love Actually etc
### Problem Definition
- Despite the abundance of movie reviews available on the internet, film studios often face challenges deriving key insights from these various data sources - primarily due to the huge volume of text data tends to be compute constraints.
### Objective
- To identify and extract subjective information from 5 Christmas movies, and helping a film studios to understand the social opinion of their movies - plot, cast, screenplay etc while monitoring online discourse.
### Data Source
 - Review data for 5 movies was harvested from IMDb, Rotten Tomatoes and Metacritic

### IDE
- google colab T4 GPU

### Concepts Applied:
-LLaMA foundation model
- Prompt Engineering
  - A prompt contains any of the following elements:

        -  **Instruction** - a specific task or instruction you want the model to perform

        - **Context** - external information or additional context that can steer the model to better responses

        -  **Input Data **- the input or question that we are interested to find a response for

        -  **Output Indicator** - the type or format of the output.

#### Optimization Parameters 

    **max_tokens**: specifies the maximum number of tokens the model should generate in response to the prompt.

     **temperature**: controls the randomness of the generated response. A higher temperature value will result in a more random response, while a lower temperature value will result in a more predictable response.

     **top_p:** This parameter controls the diversity of the generated response by establishing a cumulative probability cutoff for token selection. A higher value of top_p will result in a more diverse response, while a lower value will result in a less diverse response.

    **top_k**: This parameter controls the maximum number of most-likely next tokens to consider when generating the response at each step.

    **repeat_penalty**: This parameter controls the penalty for repeating tokens in the generated response. A higher value of repeat_penalty will result in a lower probability of repeating tokens, while a lower value will result in a higher probability of repeating tokens.

    **stop**: This parameter is a list of tokens that are used to dynamically stop response generation whenever the tokens in the list are encountered.

    **echo**: This parameter controls whether the input (prompt) to the model should be returned in the model response.

     **seed: This parameter specifies a seed value that helps replicate results.
