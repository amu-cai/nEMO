# nEMO: Dataset of Emotional Speech in Polish

## Overview

nEMO is a simulated dataset of emotional speech in the Polish language. The corpus contains over 3 hours of samples recorded with the participation of nine actors portraying six emotional states: anger, fear, happiness, sadness, surprise, and a neutral state. The text material used was carefully selected to represent the phonetics of the Polish language. The corpus is available for free under the Creative Commons license (CC BY-NC-SA 4.0).

## Content

Inside the `samples` folder, you'll find audio files named according to the `file_id` attribute listed in `data.tsv`. This TSV file contains attributes for each audio sample, including:

- `file_id` - filename, i.e. `{speaker_id}_{emotion}_{sentence_id}.wav`,

- `emotion` - label corresponding to emotional state,

- `raw_text` - original (orthographic) transcription of the audio,

- `normalized_text` - normalized transcription of the audio,

- `speaker_id` - id of speaker,

- `gender` - gender of the speaker,

- `age` - age of the speaker.

## Usage

To work with the nEMO dataset on GitHub, you may clone the repository and access the files directly within the `samples` folder. Corresponding metadata can be found in the `data.tsv` file.

The nEMO dataset is provided as a whole, without predefined training and test splits. This allows researchers and developers flexibility in creating their splits based on the specific needs.

## Supported Tasks

- **Audio classification:** This dataset was mainly created for the task of speech emotion recognition. Each recording is labeled with one of six emotional states (anger, fear, happiness, sadness, surprised, and neutral). Additionally, each sample is labeled with speaker id and speaker gender. Because of that, the dataset can also be used for different audio classification tasks.
- **Automatic Speech Recognition:** The dataset includes orthographic and normalized transcriptions for each audio recording, making it a useful resource for automatic speech recognition (ASR) tasks. The sentences were carefully selected to cover a wide range of phonemes in the Polish language.
- **Text-to-Speech:** The dataset contains emotional audio recordings with transcriptions, which can be valuable for developing TTS systems that produce emotionally expressive speech.

## Additional Information

### Licensing Information

The dataset is available under the Creative Commons license (CC BY-NC-SA 4.0).

### Citation Information

You can access the nEMO paper at [ACL Anthology](https://aclanthology.org/2024.lrec-main.1059/). Please cite the paper when referencing the nEMO dataset as:

```
@inproceedings{christop-2024-nemo-dataset,
    title = "n{EMO}: Dataset of Emotional Speech in {P}olish",
    author = "Christop, Iwona",
    editor = "Calzolari, Nicoletta  and
      Kan, Min-Yen  and
      Hoste, Veronique  and
      Lenci, Alessandro  and
      Sakti, Sakriani  and
      Xue, Nianwen",
    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
    month = may,
    year = "2024",
    address = "Torino, Italia",
    publisher = "ELRA and ICCL",
    url = "https://aclanthology.org/2024.lrec-main.1059",
    pages = "12111--12116",
    abstract = "Speech emotion recognition has become increasingly important in recent years due to its potential applications in healthcare, customer service, and personalization of dialogue systems. However, a major issue in this field is the lack of datasets that adequately represent basic emotional states across various language families. As datasets covering Slavic languages are rare, there is a need to address this research gap. This paper presents the development of nEMO, a novel corpus of emotional speech in Polish. The dataset comprises over 3 hours of samples recorded with the participation of nine actors portraying six emotional states: anger, fear, happiness, sadness, surprise, and a neutral state. The text material used was carefully selected to represent the phonetics of the Polish language adequately. The corpus is freely available under the terms of a Creative Commons license (CC BY-NC-SA 4.0).",
}
```

### Contributions

Thanks to [@iwonachristop](https://github.com/iwona-christop) for adding this dataset.
