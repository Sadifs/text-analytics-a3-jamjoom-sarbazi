Reflection — Student B (Aziza Jamjoom)

What I Learned  
This assignment gave me a much deeper understanding of NMF (Non-negative Matrix Factorization) as an unsupervised topic modeling technique. Compared to LDA, I learned that NMF focuses more on decomposing the document-term matrix into interpretable components, where each topic is a combination of words with non-negative weights. This made the topics feel more distinct and easier to interpret in some cases.  

I also learned how preprocessing decisions directly impact topic quality. Using TF-IDF instead of raw counts changed how important words were weighted, and tuning parameters like k (number of topics) played a big role in how specific or general the topics appeared. I became more comfortable understanding how to evaluate topic quality not just numerically, but based on interpretability and clarity of themes.

On the technical side, I improved my ability to work with TF-IDF vectorization, NMF modeling in sklearn, and managing outputs across multiple files. I also learned how to organize results (topics, prevalence, and top documents) and use them together to build meaningful interpretations.

Challenges  
The most challenging part of this assignment was interpreting the topics. While the model outputs top words, those words were sometimes too generic or overlapping across topics. This meant I had to rely heavily on the top documents to understand the true meaning of each topic. Translating that into a clear and specific label required careful reading and judgment.

Another challenge was managing files and debugging in Google Colab. I ran into multiple issues with file paths and loading results across notebooks, especially when working with saved CSV outputs. Fixing these issues took time and required me to better understand how the notebook environment handles file directories.

Comparing topics across California, Paris, and Hong Kong was also challenging but insightful. Some themes were consistent across parks (such as queues and pricing), while others were more location-specific. Interpreting these differences required me to think more critically about context rather than just relying on the model outputs.

Time management was also difficult. The assignment required multiple steps including modeling, saving outputs, loading results, and interpretation. The interpretation section in particular took much longer than expected because it required detailed reading and writing for each topic.

Peer Evaluation  
The collaboration process worked well overall. As a group, we aligned early on how to divide the work between LDA and NMF approaches. My teammate focused on LDA while I worked on NMF, which allowed us to explore two different modeling techniques on the same dataset.  

We worked independently on our respective parts and then reviewed each other’s work to ensure consistency in structure and presentation. This made the final project feel cohesive while still allowing each of us to contribute our own analysis.

Overall Reflection  
This was one of the most challenging assignments because of how open-ended it was. Unlike supervised learning, there is no single “correct” answer in topic modeling. Instead, it requires interpretation, judgment, and the ability to explain results clearly.  

Through this project, I feel more confident working with unstructured text data and applying topic modeling techniques like NMF. More importantly, I improved my ability to take model outputs and turn them into meaningful insights, which is a key skill in real-world data analysis.
