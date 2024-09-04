# multilingual-sarcasm-analysis
### **ABSTRACT**
A groundbreaking multilingual and multimodal sentiment and sarcasm analysis system is poised to revolutionize social media analytics. Unlike current NLP methods primarily focused on mainstream languages like English, our solution extends its scope to include regional languages such as Telugu, addressing a crucial gap in the field. Traditional methods often lack robust training on sarcastic datasets, hindering accurate sentiment analysis. Sarcasm analysis, integral to understand customer satisfaction, brand assessment, and product awareness, necessitates extensive training and testing for optimal accuracy. The proposed methodology integrates emotion detection and multimodal analysis, encompassing text and image sentiment analysis using pre-trained transformer models, offering a comprehensive approach to understand user sentiments. Leveraging these outputs, the  solution generates creative dashboards for enhanced analysis and comprehension, empowering businesses to make informed decisions in today's dynamic social media landscape.

### **AIM**
This project aims to develop an advanced sentiment and sarcasm analysis system for social media discourse, addressing the growing volume of diverse language data and the increasing demand for robust analytics in business decision-making.

### **Motivation**
1. Acknowledging the exponential growth of social media with over 4.66 billion active users worldwide.
2. Recognizing the expansion of online conversations in languages beyond English, emphasizing the importance of sophisticated sentiment analysis tools.
3. Objective is to empower businesses with actionable insights derived from diverse linguistic contexts.
4. Goal is to facilitate informed decision-making processes for businesses operating in multilingual environments.

### **INTRODUCTION**

 The emergence of online communication and expression of thoughts in the world wide web (platforms such as twitter, reddit etc) has compelled us to understand sentimen expressed through texts and emojis. Among nuances of online discourse, sarcasm stands as an emotion which is particularly tough to interpret especially by the processing models. In the recent years there has been a significant increase in multi-language content on social media and this clearly explains that there is an evident need for robust sarcasm detection and classification on different languages by understanding on how the statement is said and not just how it is said. Existing techniques typically rely on lexical and syntactic features to identify sentiment polarity, overlooking the nuanced linguistic cues indicative of sarcasm. ”Remarks that mean the opposite of what they say, made to criticize someone or something in a way that is amusing to others but annoying to the person criticized” as quoted in the Cambridge dictionary clearly explains the complexities of sarcasm as it requires an approach that goes beyond the existing unimodal analysis. This points to the manuscriotcritical need of advancement in model architecture as well as dataset to understand sarcasm in English
 as well as Telugu languages.
 The use of dravadian languages is increasing significantly in the social media platforms and Telugu is one of the national languages in india with significant number of speakers. Telugu language for sarcasm contributes to the vast potential for sarcasm analysis that has been relatively untapped until now. We have also incorporated English as it is a global language.By harnessing the power of pre-trained transformer models, analyzing the textual content and visual elements such as emojis, our methodology is proposed to offer comprehensive perspective of user sentiment across cultures and enhance the capability of sarcasm detection systems by enabling a nuanced interpretation of sentiment that aligns more closely with human judgment.
 ### **Basic Models** 
**BERT**
 BERT, which stands for Bidirectional Encoder Representations from Transformers, is based on transformers, a deep learning model in which every output element is connected to every input element, and the weightings between them are dynamically calculated based upon their connection. The BERT model is finetuned to effectively capture linguistic nuances and contextual cues specific to sarcasm across multiple languages, including English and Telugu.
**Indic BERT**
 IndicBERT is a language model designed specifically for understanding and processing various Indian languages. Like its predecessor BERT, it uses a transformer architecture to read and understand entire sentences at once, but it’s tailored to handle the linguistic nuances and diversity of Indian languages. This includes languages like Hindi, Bengali, Tamil, Telugu, and many others. Indic BERT is specifically trained on diverse languages, including Hindi, Telugu, Tamil, Bengali, and others, making it particularly suited for analyzing sarcasm in multilingual contexts. Through fine-tuning Indic BERT on sarcasm labeled datasets in various Indic languages, it can be optimized in terms of its performance for detecting sarcastic expressions.
 **TF-IDF**
 TF-IDF (Term Frequency-Inverse Document Frequency) played a pivotal role in preprocessing textual data and extracting features for sarcasm detection. TF-IDF, a fundamental technique in natural language processing, enabled us to represent each sentence as a numerical vector based on the frequency of its constituent words across the dataset, while also considering their importance in distinguishing between sarcastic and non-sarcastic expressions. By computing the TF-IDF scores for words in the dataset, we obtained a high-dimensional feature space that captured the unique linguistic characteristics associated with sarcasm.


Positive Sarcasm: "This is definitely the best product ever... if you enjoy waiting forever for it to arrive."
Negative Sarcasm: "I'm thrilled to spend my entire weekend doing paperwork."

Basic Model Architechture:
 [Input] -> [Word Embedding] -> [Transformer] -> [Attention] -> [Sarcasm Detection] -> [Output]

### **GAP ANALYSIS**

1. Most of the studies have involved the usage of only 1 language in their models and only for Hindi there exists a code mixed language along with english.
2. Methods that were developed from machine learning suffer from contextual gaps .
3. And some of the models have used  predefined input structures(like ques and ans model, max length etc..) for analysis . They cannot be applicable on real time data from social media websites.
4. Humor detection models using different versions of language Models like bert cannot work for sarcasm analysis. And also the dataset is extracted from single source.
5. Emoji extraction for multimodal analysis , alongside Telugu language is not done.

### **SCRUM MODEL**


![image](https://github.com/user-attachments/assets/bf1df359-4aae-4bbc-a34f-e8219935d119)
