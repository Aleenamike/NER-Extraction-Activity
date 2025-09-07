# Named Entity Recognition (NER) Project

## 📌 CADL Activity 3

### 🔹 Task
- Use a **pre-trained spaCy NER model** on a text dataset (job postings).  
- Identify **named entities** like `PERSON` and `ORG`.  
- Extract structured information in a table format.  

---

### 🛠️ Requirements
- Python 3.x  
- Libraries:  
  ```bash
  pip install spacy pandas
  python -m spacy download en_core_web_sm

Example Dataset (Job Postings)
1. Google is hiring Data Scientists in Bangalore. Contact John Doe for details.
2. Microsoft announced new AI research positions in Hyderabad, reach out to Jane Smith.
3. Amazon is looking for Software Engineers in Seattle.
4. Infosys offered a Project Manager role in Pune, supervised by Rahul Kumar.

Run the Program
python ner_extraction.py

Expected Output
Named Entities Identified:
Google -> ORG
Bangalore -> GPE
John Doe -> PERSON
Microsoft -> ORG
Hyderabad -> GPE
Jane Smith -> PERSON
Amazon -> ORG
Seattle -> GPE
Infosys -> ORG
Pune -> GPE
Rahul Kumar -> PERSON

Structured Table (Persons & Organizations):

Sentence	               Entity	      Label
Google is hiring...	     Google	      ORG
Google is hiring...	     John Doe	    PERSON
Microsoft announced...	 Microsoft    ORG
Microsoft announced...	 Jane Smith  	PERSON
Amazon is looking...	   Amazon	      ORG
Infosys offered...	     Infosys	    ORG
Infosys offered...	     Rahul Kumar	PERSON
