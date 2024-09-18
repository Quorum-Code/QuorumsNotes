
# Cannot be rated

## Non-coding questions
* Questions outside the scope of the model

## Personal Info
* Full names, personal info
* Literal directories
* Non-English prompts

# Correctness

## Major Issues
* Incorrect text/explanations, logical errors in code
* Non-functional code

## Minor Issues
* Factual claims in text but some inaccuracies in details
* Code has inefficiency or incorrect comments

## Cannot Assess
* Cannot determine validity of claims
* Response is a punt (Hallucinations, such as I am a large-language model and can't write code.)

## Not Applicable
* No explicit or implicit claims are made in the response and it doesn't contain code

## Mistake in code comments
* Incorrect iterator notation
## Mistake in text/explanations
* Bad links

# Instruction Following

## Major Issues
* Missed key components of the prompt making the response unhelpful

## Minor Issues
* Misinterpreted small parts of the prompt

## Not applicable
* No explicit or implicit instructions to follow or the response is canned 
* or the response is a punt (As an AI model I am not capable of responding to this type of question)

# Misc.

## Verbosity
* If responses are about equal prefer the more concise

## Running Code
* Do not penalize code for missing context which may be required to run, i.e. a main function to test the function
* All code blocks should be tested
* DONT CHANGE THE LOGIC OF THE CODE WHEN TESTING