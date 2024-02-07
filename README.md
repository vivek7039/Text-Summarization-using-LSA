# Text-Summarization-using-LSA
Extractive text summarization using Latent Semantic Analysis (LSA)

Extractive text summarization is a technique used to generate a concise summary of a document by selecting and extracting key sentences or phrases directly from the original text. Unlike abstractive summarization, which involves generating new sentences to convey the essential meaning, extractive summarization relies on identifying and extracting existing content.

In our extractive text summarization approach for financial documents, we are implementing Latent Semantic Analysis (LSA) to identify and extract key information. LSA helps us uncover hidden relationships between words and sentences, enabling a more nuanced understanding of the content. Our analysis is specifically applied to the FNS-2021 Shared Task: [“Financial Narrative Summarisation”](https://wp.lancs.ac.uk/cfie/fns2021/), ensuring that our summarization model is  evaluated on a comprehensive collection of financial documents. This approach leverages LSA's capability to capture semantic relationships, enhancing the accuracy and relevance of the extracted summaries for financial texts within the designated dataset.

In our extractive text summarization study focused on financial documents, we conducted evaluations using the ROUGE (Recall-Oriented Understudy for Gisting Evaluation) score on the provided validation dataset. This metric allowed us to quantitatively assess the performance of our summarization model by measuring the overlap between the generated summaries and the reference summaries in the validation set. The use of ROUGE scores provides a comprehensive evaluation framework, considering precision, recall, and F1-score, ensuring that our extractive summarization approach is robust and aligns with the content of the financial documents present in the specified dataset.

In addition to employing the ROUGE score for evaluation, we utilized a Java-based open-source evaluator to assess our extractive text summarization model. This evaluator generated a result.csv file containing detailed evaluation metrics. The evaluator can be found [here](https://github.com/kavgan/ROUGE-2.0).

Also, the entire FNS dataset can be accessed [here](https://drive.google.com/file/d/1o7iW-cpIXCpQI7mNaYJ4T-2vQOwgRbVw/view).

The complete file takes time to run. If you want to see a demo you can use the toy dataset and toy file included in the repository.

STEPS:

Running Locally

1. Upload the zip of validation dataset on drive
2. Comment out the import statement for google colab and the code in cell below "use_colab=False"
3. Using the summaries generated in the gen_sum folder use JAVA tool to evaulate the rouge score which will be a result.csv file.
5. Place the file in the Text-Summarization-using-LSA folder outside all folders.
6. Check for the rouge scores.


Running on COLAB

1. Upload the zip of validation dataset on drive
2. Uncomment import statement for google colab and the code in cell below "use_colab=False"
3. After running the cell set the "dataset_path" of the folder where the validation zip is uploaded.
4. Using the summaries generated in the gen_sum folder use JAVA tool to evaulate the rouge score which will be a result.csv file.
5. Place the file in the Text-Summarization-using-LSA folder outside all folders.
6. Check for the rouge scores.

