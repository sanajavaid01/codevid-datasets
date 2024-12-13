# Dataset for Programming-based Instructional Videos Classification and Question Answering

## Abstract

This work aims to develop an understanding of the rapidly emerging field of VideoQA, particularly in the context of instructional programming videos. It also encourages designing systems that can produce visual answers to programming-based natural language questions.

We introduce two datasets:

1. **CodeVidQA**: Contains 2,104 question-answer pair links with timestamps taken from programming videos of Stack Overflow for the Programming Visual Answer Localization task.
2. **CodeVidCL**: Comprises 4,291 videos (1,751 programming and 2,540 non-programming) for the Programming Video Classification task.

In addition, we propose a framework that adapts BigBird and SVM for video classification techniques. The proposed approach achieves a significantly high accuracy of 99.61% for video classification.

## Repository Contents

This repository contains:

- **Datasets (Excel Sheets)**: The `datasets/` folder includes Excel sheets for CodeVidQA and CodeVidCL. These files contain detailed information about the datasets and their annotations.
- **README.md**: Documentation and guidelines for using the repository.

## Datasets

1. **CodeVidQA Dataset**:

   - Includes 2,104 question-answer pair links.
   - Each pair contains:
     - A natural language question.
     - The corresponding visual answer localized with timestamps.

2. **CodeVidCL Dataset**:
   - Contains 4,291 videos labeled for classification:
     - 1,751 programming videos.
     - 2,540 non-programming videos.

The datasets are provided as Excel sheets located in the `datasets/` folder.

## How to Use the Datasets

1. Clone the repository:

   ```bash
   git clone https://github.com/sanajavaid01/codevid-datasets
   cd dataset-videoqa
   ```

2. Navigate to the `datasets/` folder to access the Excel sheets.

3. Load the datasets using your preferred data analysis tools or libraries, such as Python's pandas:

   ```python
   import pandas as pd

   codevidqa = pd.read_excel("datasets/Code_Vid_QA_Dataset.xlsx")
   codevidcl = pd.read_excel("datasets/Code_Vid_CL_Dataset.xlsx")
   ```

## Framework for Video Classification

The proposed framework adapts the following techniques:

- **BigBird**: A transformer model optimized for long sequences, used for encoding.
- **SVM (Support Vector Machine)**: Utilized for classification tasks.

Our framework achieves an accuracy of 99.61% for classifying programming and non-programming videos.

<!-- ## Citation
If you use this dataset or framework in your research, please cite:

```
@article{yourcitation2024,
  title={Dataset for Programming-based Instructional Videos Classification and Question Answering},
  author={Your Name and Collaborators},
  journal={Your Journal},
  year={2024},
}
``` -->

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

We would like to thank Stack Overflow for providing the videos and the research community for their continuous support.

---

Feel free to raise an issue or submit a pull request if you have any suggestions or questions!
