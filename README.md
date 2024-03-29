# CSC413Project
The course project for CSC413 2024S

## Project Target
- Create an NLP model such that user enter job description and exerience in natural language, and output range of salary (Classification)

## Links
#### Dataset:
- https://www.kaggle.com/datasets/jaiganeshnagidi/data-scientist-salary?resource=download
#### How-to's
- how to fine tune using bert: https://huggingface.co/docs/transformers/training

## Ideas
- Use bert as pre-trained model, train with training dataset descriptions.
- Discard job-category | company name; Keep job-description | job-requirements | experience category 

## Steps
### Preprocessing Data
- Remove unnecessary columns.
- Re-categorize experience and salary.
- Tokenize Natural Language inputs.
### Model Building
- Concatenate "experience", "job_location", "job_desig", "key_skills", "job_description"
- Use "Salary" as target.
- Fine-Tune BERT by adding a linear layer and train the last epoch with our training data and target.
- Use Bert Pre-trained model
- No decoder, directly output a class
### Compare With Naive RNN
- Hand code RNN, 2 version encoding
  - Word2Vec version
  - BERT feature version
- Compare output of same test inputs
### Report
- 6-8 page report.

## Timeline
### Week March 25-31
- Prepare Data
- Draft Fine-tune version
### Week April 1-7
- RNN versions
- Comparison
### Week April 8-15
- Report
