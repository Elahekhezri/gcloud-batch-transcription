# gcloud-batch-transcription
# Overview

This script transcribes batches of audio files using Google Cloud's Speech-to-Text API. It then automatically structures the data into a pandas DataFrame with filenames and corresponding transcriptions.

☀️ Recommended for qualitative researchers transcribing audio interviews or survey voice notes.

☀️ Recommended for audio files in languages not widely supported by online batch transcription tools (e.g., Persian). 

💡 For the final dataframe to be analysis-ready:
- Name audio files after participant IDs.

- Name folders after research variables or conditions.


# Setup

## 🏗️ Environment:
- [Google Colab](https://colab.research.google.com/) (Recommended, minimal setup).
- If running locally, authentication setup may differ.

## 🗃️ Storage
- Google Cloud Storage Bucket (easy integration with Google Cloud Speech-to-Text)
- ⚠️ Tweak the code to pull audio from other sources if you're not using storage bucket.

## Prep

1. Go to [Google Cloud Console](https://console.cloud.google.com/).
2. Create a new project or select an existing one.
3. Enable [Cloud Speech-to-Text API](https://console.cloud.google.com/apis/library/speech.googleapis.com?) for the project.
4. (optional) Enable [Cloud Storage API](https://console.cloud.google.com/apis/library/storage-component.googleapis.com?) for the project -> Go to [Cloud Storage Buckets](https://console.cloud.google.com/storage/) -> create a bucket -> upload the folder containing the audio files.
5. (optional) Depending on your authentication method, you may need to [create a service account](https://cloud.google.com/iam/docs/service-accounts-create).

# ⚠️ Warning
As of Summer 2024, this script ran at no cost. However, Google Cloud pricing may change, so check the latest terms before use.

# Code

You can find the full transcription script in the repo: [batch_transcription_gcloud_speech_to_text.ipynb](batch_transcription_gcloud_speech_to_text.ipynb)

Or, run it directly in Google Colab: [colab notebook](https://colab.research.google.com/drive/1lFz0DOkhqIpX85Ddb3haEDC-XjQQBKnD?usp=sharing)


