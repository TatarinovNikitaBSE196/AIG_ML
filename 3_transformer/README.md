Based on [this article](https://doi.org/10.48550/arXiv.1908.08594) - retraining [GPT-2](https://github.com/nshepperd/gpt-2).  
Download [retrained model](https://drive.google.com/file/d/1TvF0ECexuH0dXVAd0No9ELk6fsOkBBdB/view?usp=sharing) and place it to *models/lecture/* directory.  
Point command line to this folder.  
To get unconditional samples, run:  
`python src/generate_unconditional_samples.py --model_name lecture`  
To get conditional samples, run:  
`python src/interactive_conditional_samples.py --model_name lecture --length 50`