# nEMO: Dataset of Emotional Speech in Polish

## Dataset Description

nEMO is a simulated dataset of emotional speech in the Polish language. The corpus contains over 3 hours of samples recorded with the participation of nine actors portraying six emotional states: anger, fear, happiness, sadness, surprise, and a neutral state. The text material used was carefully selected to represent the phonetics of the Polish language. The corpus is available for free under the Creative Commons license (CC BY-NC-SA 4.0).

### Example Usage

The nEMO dataset can be loaded and processed using the datasets library:

```python
from datasets import load_dataset

nemo = load_dataset("amu-cai/nEMO", split="train")
```

### Supported Tasks

- `audio-classification`: This dataset was mainly created for the task of speech emotion recognition. Each recording is labeled with one of six emotional states (anger, fear, happiness, sadness, surprised, and neutral). Additionally, each sample is labeled with speaker id and speaker gender. Because of that, the dataset can also be used for different audio classification tasks.
- `automatic-speech-recognition`: The dataset includes orthographic and normalized transcriptions for each audio recording, making it a useful resource for automatic speech recognition (ASR) tasks. The sentences were carefully selected to cover a wide range of phonemes in the Polish language.
- `text-to-speech`: The dataset contains emotional audio recordings with transcriptions, which can be valuable for developing TTS systems that produce emotionally expressive speech.

### Languages

nEMO contains audio and transcription in Polish language.

## Dataset Structure

### Data Instances

```python
{
  'audio': {
    'path': None,
    'array': array([ 6.10351562e-05, -3.05175781e-05, -3.05175781e-05, ...,
      6.10351562e-05, -1.22070312e-04,  1.83105469e-04]),
    'sampling_rate': 24000
  },
  'emotion': 'surprised',
  'raw_text': 'Ucho wykrywa dźwięki o różnej częstotliwości.',
  'normalized_text': 'ucho wykrywa dźwięki o różnej częstotliwości',
  'speaker_id': 'WR0',
  'gender': 'male',
  'age': '23'
}
```

### Data Fields

- `audio` (audio) - dictionary containing audio array, path and sampling rate,
- `emotion` (string) - label corresponding to emotional state,
- `raw_text` (string) - original (orthographic) transcription of the audio,
- `normalized_text` (string) - normalized transcription of the audio,
- `speaker_id` (string) - id of speaker,
- `gender` (string) - gender of the speaker,
- `age` (string) - age of the speaker.

### Data Splits

The nEMO dataset is provided as a whole, without predefined training and test splits. This allows researchers and developers flexibility in creating their splits based on the specific needs.

## Additional Information

### Licensing Information

The dataset is available under the Creative Commons license (CC BY-NC-SA 4.0).

### Citation Information

You can access the nEMO paper at [link]. Please cite the paper when referencing the nEMO dataset as:

```
@article{}
```

### Contributions

Thanks to [@iwonachristop](https://github.com/iwona-christop) for adding this dataset.