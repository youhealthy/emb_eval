# Word embedding evaluation

And vector represented word embedding can be evaluated for different tasks. E.g. word similarity, word analogy, doc representation etc.

Currently support
1. word similarity evalution
Use human labelled similarity score between select word, compare similarity score generated by embedding vector. The closer to human similarity score, the closer to human judgement.

2. doc classification evaluation
Represent doc using a combination of word embedding. The easiest way is to average (too naive). Can use RNN to generate better representation. Use representation and doc embedding to classify.

run

> python scripts/evaluate_word_embedding.py --out_dir=output/eval --emb_path=/tmp/glove.twitter.27B.100d.txt --csv_separator=" " --quoting=3
