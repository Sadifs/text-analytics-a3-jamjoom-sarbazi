# Reflection — Student A (Sadaf Sarbazi)

---

## What I Learned

This assignment gave me a much deeper understanding of LDA (Latent Dirichlet Allocation) as an unsupervised topic modeling technique. Unlike Assignments 1 and 2 where the labels were given, here I had to discover structure in the data myself, which was a genuinely different kind of challenge. I learned how LDA represents documents as mixtures of topics, and topics as distributions over words and how hyperparameters like k, min_df, and max_iter affect the quality of the output. I also learned that coherence score is a better guide for topic quality than perplexity, and that informal user-generated text like Disneyland reviews will naturally produce lower coherence scores than formal corpora, which initially worried me but turned out to be expected and normal.

On the technical side, I got much more comfortable with the sklearn LDA pipeline, CountVectorizer, and the preprocessing decisions that go into building a clean corpus. The preprocessing experiments (comparing unigrams vs bigrams and different min_df thresholds) taught me that small configuration choices can meaningfully affect topic interpretability.

---

## Challenges

Topic interpretation was the most time-consuming and demanding part. Reading top words alone was not enough as I had to read representative documents per topic, identify recurring patterns, and translate that into a specific, meaningful name. Doing this for 15 topics across 3 parks took much longer than I expected. There were moments where the top words were generic and did not obviously point to a clear theme, which required careful reading of the actual reviews to understand what the model had captured.

Coherence scores were a source of difficulty and uncertainty. All scores fell in the 0.42–0.46 range, sitting just below the 0.5 "good" threshold in the rubric. I spent significant time attempting to push scores above 0.5 by testing different configurations — switching from bigrams to unigrams, lowering min_df, increasing max_iter, switching to batch learning, and extending the k range to {5, 8, 10, 12, 15, 20, 25, 30}. Despite these efforts, scores remained below 0.5 for all three parks. After confirming with the professor that this range is acceptable for informal user-generated review text, I understood that coherence thresholds in the rubric are benchmarks for formal corpora, and that published topic modeling work on Amazon and Yelp reviews reports similar ranges.

pyLDAvis was unexpectedly difficult. The library had compatibility issues with my Python 3.13 environment, the standard import path did not work, and it took multiple attempts and version checks to get the HTML exports working. Once I understood that the prepare() function required specific arguments (topic-term distributions, doc-topic distributions, term frequencies), it clicked — but it was a frustrating debugging process.

Time management was also a challenge. This assignment has many moving parts (EDA, preprocessing, modeling, evaluation, interpretation, and documentation) and it was easy to underestimate how long each step would take. I ended up spending significantly more time than anticipated, particularly on the interpretation section.

---

## Peer Evaluation 

---

## Overall Reflection

This was the most open-ended assignment of the three, and the most challenging because of it. Supervised learning feels more structured as you have a target, you optimize toward it, you evaluate with clear metrics. Unsupervised learning requires judgment at every step: how many topics, which words to remove, what a topic actually means. That judgment is harder to develop but more valuable in practice. I feel more confident now in my ability to apply topic modeling to a real business problem and explain what the results mean to a non-technical audience.
