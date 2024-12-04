# Multilingual Text Classification Dataset

## Overview
This dataset contains **138,813 text entries** curated for tasks such as text classification, spam detection, and multilingual analysis. Each entry includes a label (e.g., "ham" for non-spam or "spam") and a text snippet. Language annotations are available for **41 unique languages**, enabling exploration of cross-linguistic patterns.

## Key Features
- **label**: Classification label (e.g., "ham" or "spam").
- **text**: The main content of the message.
- **lang**: Language code (ISO 639-1 format) for a subset of the data.
- **URL, EMAIL, PHONE**: Binary indicators for the presence of URLs, emails, or phone numbers.
- Sparse and unnamed columns are present but can be ignored for most tasks.

## Statistics
- **Total Entries**: 138,813
- **Unique Languages**: 41
- **Most Common Language**: English (detailed distribution in the language summary file).

## Potential Use Cases
1. **Multilingual NLP**: Training multilingual models for classification or sentiment analysis.
2. **Spam Detection**: Evaluating models on spam/non-spam detection tasks.
3. **Language Identification**: Investigating patterns across diverse languages.

## File Structure
The dataset includes the following columns:
| Column       | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| `label`      | Classification label (`ham` or `spam`).                                    |
| `text`       | Message content (text data).                                               |
| `lang`       | Language of the message (ISO 639-1 format).                                |
| `URL`        | Indicates the presence of URLs in the message (`Yes`/`No`).                |
| `EMAIL`      | Indicates the presence of email addresses in the message (`Yes`/`No`).     |
| `PHONE`      | Indicates the presence of phone numbers in the message (`Yes`/`No`).       |
| Other Columns| Sparse columns (can be ignored for most tasks).                            |

## Language Distribution
A breakdown of the language annotations is provided in the `Language_Count_Summary.csv` file. This file contains:
- Language code.
- Number of entries for each language.

## Getting Started
1. **Download the dataset**: Clone this repository or download the dataset directly.
2. **Load the dataset**: Use Python libraries like `pandas` to load and analyze the data.

   ```python
   import pandas as pd
   
   # Load the dataset
   data = pd.read_csv('path_to_dataset.csv')
   print(data.head())
