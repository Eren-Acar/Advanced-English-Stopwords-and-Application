import nltk
from nltk.corpus import stopwords
nltk.download('stopwords')


df = "Example dataframe"

stop_words = set(stopwords.words('english') + [
    'cant', 'dont', 'even', 'get', 'go', 'going', 'im', 'ive', 'like', 'really', 'want',
    'also', 'anyone', 'back', 'would', 'things', 'one', 'much', 'feeling', 'got', 'know',
    'never', 'since', 'always', 'something', 'started', 'still', 'take', 'anything', 'could',
    'getting', 'last', 'think', 'else', 'every', 'everything', 'lot', 'make', 'way', 'ago',
    'better', 'didnt', 'see', 'someone', 'went', 'well', 'thoughts', 'well', 'trying', 'first',
    'right', 'thought', 'person', 'ever', 'self', 'without', 'best', 'looking', 'day', 'ever',
    'broke', 'without', 'best', 'looking', 'ever', 'said', 'shes', 'hes', 'made', 'talk', 'tell',
    'thing', 'days', 'away', 'around', 'try', 'thats', 'times', 'saying', 'wasnt', 'doesnt', 'say',
    'wanted', 'nothing', 'anymore', 'keep', 'two', 'point', 'let', 'makes', 'asked', 'talking',
    'normal', 'actually', 'come', 'sure', 'many', 'done', 'find', 'though', 'end', 'left', 'deal',
    'maybe', 'stop', 'give', 'whats', 'etc', 'almost', 'little', 'everyone', 'tired', 'long', 'post',
    'id', 'able', 'another', 'says', "i", "am", "did", "does", "do", "was", "were", "will", "are", "be", "been", 
    "being", "have", "has", "had", "having", "shall", "should", "would", "may", "might", "must", "can", "could", 
    "ought", "dare", "need", "used", "seem", "see", "look", 
    "appear", "sound", "smell", "taste", "feel", "become", "get", "grow", "turn", "prove", "remain","removed", "deleted",
    "ampx200b",
    "asks", "told", "oh", "put", "next"
])


punctuations = "!\"#$%&()*,-./:;<=>?@[\\]^_`{|}~'"
pattern = r'\b(?:' + '|'.join(stop_words) + r')\b'

df['example_column_cleaned'] = df['example_column'].str.lower()

# remove stopwords
df['example_column_cleaned'] = df['example_column_cleaned'].str.replace(pattern, '', regex=True)


# remove punctuations
df['example_column_cleaned'] = df['example_column_cleaned'].str.replace('[{}]'.format(punctuations), '', regex=True)
