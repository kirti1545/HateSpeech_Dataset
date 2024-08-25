# HateSpeech_Dataset

Our research was accepted at ICPR 2024, where we showed the effectiveness of Multimodality in detecting hate speech. we have generated both hate and non-hate speech samples by transforming text excerpts from the ToxiGen dataset into audio representations.  1000 random text samples belonging to both hate and non-hate classes are selected to generate the audio samples, comprising 502 non-hate sentences and 498 hate sentences. We utilized the Speech T5 pre-trained model to transform the text into audio, achieving seamless conversion through advanced language processing techniques.  Within the SpeechT5 framework, various speakers are available, including two distinct male voices, BDL and RMS, and two female voices, CLB and KSP, along with a Surprise Me! voice. To ensure a comprehensive evaluation, we generated the audio dataset using four distinct voices: two male voices (BDL and RMS) and two female voices (CLB and KSP). We utilized both the male voices, BDL and RMS, and generated 1,000 audio samples for each using a specific set of texts. Similarly, employing the same set of 1,000 texts, we generated audio using the CLB and KSP female voices.

#### Dataset Details
| **Voices**    | **No of samples** |
|-----------|---------------|
|Male (BDL) |   1000        |
|Male (RMS) |   1000        |
|Female(CLB)|   1000        |
|Female(KSP)|   1000        |

```HateSpeech_Dataset.zip``` contains the following files.
- ```text_data+labels.csv``` (contains text sentences, their labels, and sentence ids)
- ```audio_labels.csv``` (contains audio filenames and their labels)
- ```audio``` folder (containing audio files).
- audio filenames have ``` output_<Gender><Voice>_<Sentence_id>.wav``` strecture. Where gender is either male or female. Voice is among BDL, RML, CLB, and KSP. Sentence_id is the id of the sentence (see ```text_data+label.csv```) for which audio is generated.

```While performing the experiments we randomly (seed=42) splitted the data into 80:20 for training and testing respectively.```

#### Dataset Link
You can download the dataset from Google Dive [link](https://drive.google.com/file/d/1lJS1wVrRpBONDio4lGQSNXXZQDMxy8QA/view?usp=sharing) (size~600Mb). The link contains a zip file that requires password for unzipping. To get the password, please follow the license agreement below.

***If you find errors while unzipping, use ```7zip``` software in windows.***

## License Agreement
- Have the license agreement reviewed and signed by an individual authorized to make legal commitments on behalf of your institution. Your institution's legal office must review and execute the license. The signature of the Director, the Registrar, or the Head of the Department with the university seal is also accepted.
- Please scan and email the executed agreement to [akagarwal@iiserb.ac.in](mailto:akagarwal@iiserb.ac.in) to receive the password for the zip files.
- If you have any questions about this dataset, please contact at [akagarwal@iiserb.ac.in](mailto:akagarwal@iiserb.ac.in) or [kirtilekhabhesra45@gmail.com](mailto:kirtilekhabhesra45@gmail.com).

## Citation:
- Kirtilekha Bhesra, Akshay Agarwal, “A Multi-Modal Framework to Counter Hate Speeches”. In IEEE International Conference on Pattern Recognition (ICPR), 2024.
- Kirtilekha Bhesra, Shivam Ashok Shukla, Akshay Agarwal, "Audio vs. Text: Identify a Powerful Modality for Effective Hate Speech Detection". In International Conference on Learning Representations (ICLR) TinyPapers, 2023.
