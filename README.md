# BERT_personality_detection
How to fine-tune a BERT classifier using the Huggingface <a href="https://huggingface.co/transformers/quicktour.html">Transformers</a> library and Keras+Tensorflow in order to detect users' personality type based on some text they have posted, according to the Myers–Briggs Type Indicator (MBTI).

The application was developed on Google Colab and is comprised of the following steps:
- ***Data preparation***: MBTI data are loaded, preprocessed and prepared according to the BERT specifications.
- ***Fine tuning of the BERT classifier***: a classification layer is stacked on top of the BERT encoder and the entire model is fine-tuned, fully exploiting the GPU support provided by Google Colab, with very low training times.
- ***Performance evaluation***: I evaluated the trained model using ROC_AUC and Accuracy metrics, achieving an AUC of 0.725 and a binary accuracy of 0.750 on the test set. ROC curves for each personality type are shown in the following:
<img src="https://github.com/rcantini/BERT_personality_detection/blob/main/results/roc_auc.png" style="margin-left: auto; margin-right: auto; width: 90%; height: 90%"/>

I also used the model for finding out my own MBTI personality.

<img src="https://github.com/rcantini/BERT_personality_detection/blob/main/results/personality.png" style="margin-left: auto; margin-right: auto; width: 90%; height: 90%"/>

For further information, I have made the Colab notebook available in this repository. The related post is available on my blog at this link: https://riccardo-cantini.netlify.app/post/personality_detection/

Moreover, if you want to know more about BERT and how to exploit it for different text classification tasks, check out my blog post: https://riccardo-cantini.netlify.app/post/bert_text_classification/

