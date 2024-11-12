# Word_Unjumbler_Project  

This project provides a tool for unscrambling jumbled words. Given an input word, the script generates all possible permutations and filters out valid English words. For each valid word found, it displays definitions to enhance understanding.  

**Features:**  
  
+ **Word Unscrambling:** Finds possible English words from a jumbled input.  
+ **Word Definitions:** Retrieves and displays definitions for each unscrambled word.  
+ **Dictionary-Based Validation:** Uses pyenchant for dictionary validation to filter only legitimate English words.    
  
**Requirements**  
Python (3.x)  
  
**Libraries:**
+ pyenchant for word validation
+ nltk for retrieving word definitions
+ itertools (built-in) for generating permutations    

**Setup**  
1. Install the required libraries:

        pip install pyenchant nltk
        If using nltk for the first time, download WordNet:
  
2. If using nltk for the first time, download WordNet:
  
        import nltk
        nltk.download('wordnet')
3. On some systems (e.g., Linux), you may need to install enchant:


        sudo apt-get update
        sudo apt-get install libenchant-2-dev
          
**Usage**  
1. Run the script:

        python unjumbler.py  
        
2. Enter the jumbled word when prompted.

**Example**

        Enter the jumbled word: LEPA
        The unjumbled word is 'PALE'
        Definitions for 'PALE':
        - Lacking intensity of color; having a pale color
        ...

**How It Works**  
+ The script generates all permutations of the input word.  
+ For each permutation, it checks if it's a valid word in the English dictionary.  
+ If valid words are found, their definitions are displayed.    
  
**Notes**  
+ Ensure you have an active internet connection to download necessary NLTK data files.  
+ This script is intended for English-language words.  
 
