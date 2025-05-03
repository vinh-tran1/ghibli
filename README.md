# CPSC 184 Final Project Studio Ghibli v. OpenAI: Ghibli Style Dectector
**Vinh Tran**

## Project Description

In March 2025, OpenAI released a viral image-generation feature allowing users to render photos “in the style of Studio Ghibli.” With just a prompt, users could “Ghiblify” their pets, political events, memes, or even historical moments. These images mimicked the warmth, stylization, and visual language of Hayao Miyazaki’s hand-drawn films, but none were made or endorsed by Studio Ghibli.

The backlash was immediate and complex. Ethically, it reignited debates over AI’s impact on creative labor. Legally, it posed a harder question: can an aesthetic “style” be protected under copyright or trademark law? And if so, how should courts treat AI-generated works that evoke, but don’t duplicate, an iconic artistic style?

This paper explores that question through both a legal analysis and technical implementation. We built a computational tool that uses a pre-trained vision model (VGG19) and OpenAI’s Contrastive Language-Image Pre-Training (CLIP) architecture to compare AI-generated Ghibli-style images with authentic stills from Studio Ghibli films. We argue that this tool provides empirical scaffolding for key IP doctrines,  namely copyright’s substantial similarity test, fair use, and trademark dilution under the Lanham Act,  and can guide future adjudications in cases involving AI aesthetic replication.


## Set Up

### Local

**Note: it is recommended to use a virtual environment for python**

```bash
# activate
$ python3 -m venv .venv
$ source .venv/bin/activate

# deactivate
$ deactivate
```

**Install packages in virtual environment**
```bash
$ pip install -r requirements.txt
```

### Google Colab

**No need for special setup, but it is important you must 1) replicate the file structure (or modify to your structure) and 2) mount to your google drive and install the CLIP library (already in the code)**

## Running the Code
To run the python notebook, just run all the cells (click play)

## Folder Structure
- `ghibli_data`
    - `ghibli_ai`: ai-generated (SORA) Ghibli images
    - `ghibli_real`: real ghibli images
- `results`: contains the csv file of the similarity results and the plot
- `similarity_test.ipynb`: main code to run the python script
