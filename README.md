# BERT_personality_detection
How to fine-tune a BERT classifier using the Huggingface <a href="https://huggingface.co/transformers/quicktour.html">Transformers</a> library and Keras+Tensorflow in order to detect users' personality type based on some text they have posted.

The application was developed on Google Colab and is comprised of the following steps:
- ***Data preparation***: MBTI data are loaded, preprocessed and prepared according to the BERT specifications.
- ***Fine tuning of the BERT classifier***: a classification layer is stacked on top of the BERT encoder and the entire model is fine-tuned, fully exploiting the GPU support provided by Google Colab, with very low trianing times.
- ***Performance evaluation***: I evaluated the trained model using ROC_AUC and Accuracy metrics, achieving an AUC of 0.725 and a binary accuracy of 0.750 on the test set. ROC curves for each personality type are shown in the following:
<img src="https://github.com/rcantini/BERT_personality_detection/blob/main/roc_auc.png" style="margin-left: auto; margin-right: auto; width: 90%; height: 90%"/>



I further tested the model by preparing some sentences, achieving very good results.

For further information, check out my blog post: https://riccardo-cantini.netlify.app/post/bert_text_classification/

