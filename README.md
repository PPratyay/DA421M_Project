# Training CLIP for Non English Captions

**Project Description**: This project fine-tunes OpenAI CLIP on the Flickr30k image-caption dataset to improve image-caption alignment and retrieval. The notebook includes data preparation, optional caption translation, training, and validation code.

**Diagram of the Proposed Model**


  

<p align="center">
  <img src="https://raw.githubusercontent.com/PPratyay/DA421M_Project/main/CLIP_Diagram.png" alt="CLIP Diagram" width="600"/>
</p>


**Files to know**
- `Clip_Implementation.ipynb`: The main Jupyter notebook containing the full implementation and training loop.

**Detailed instructions to run the code (Kaggle)**
- **Step 1 — Upload notebook to Kaggle**:
  - Go to `https://www.kaggle.com/` and sign in.
  - From your profile, click `New Notebook` and then use `Upload` to upload `Clip_Implementation.ipynb`, or create a new notebook and copy the cells from your local notebook.

- **Step 2 — Add the Flickr30k dataset to the notebook**:
  - In the notebook editor, open the right-side pane and click `Add data` → `Upload data`.
  - Upload the Flickr30k images and the labels/results CSV the notebook expects.
  - When uploading, name the dataset `flickr-image-dataset` (or note the dataset slug) so the notebook code referencing `/kaggle/input/flickr-image-dataset/...` will work without edits.



- **Step 3 — Install dependencies (run first cells)**:
  - Run the first code cell that installs Python packages. The notebook includes lines like:

    `! pip install ftfy regex tqdm`

    `! pip install git+https://github.com/openai/CLIP.git`

  - Ensure that The Internet is enabled.

- **Step 4 — Attach dataset and run all cells**:
  - Make sure the uploaded dataset is attached to the notebook (the `Add data` panel shows the dataset attached).
  - Run all cells in order (`Runtime` → `Run all` or `Run` menu). The notebook handles preprocessing, optional translation, dataset copying into `/kaggle/working/`, DataLoader setup, training and validation loops.


