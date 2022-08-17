# Enhancing Rhyming Abilities of Neural Models for Lyrics Generation
This is my MSc Project with Huawei. The project name is "Enhancing Rhyming Abilities of Neural Models for Lyrics Generation".

## Download the data
The data used in this project is from [Chinese Lyric Corpus](https://github.com/gaussic/Chinese-Lyric-Corpus).
We need to download the zip file and unzip it as a large *Chinese_Lyrics* folder with 494 small folders indicated by the artists'names.
Then we can use the [preprocess.py](https://github.com/dbiir/UER-py/blob/master/preprocess.py) to preprocess the data into a text file using the codes below.
```
python3 preprocess.py --corpus_path corpora/lyric.txt \
                      --vocab_path models/google_zh_vocab.txt \
                      --dataset_path lyric_dataset.pt --processes_num 32 \
                      --seq_length 512 --target lm
```

## Prepare the data
