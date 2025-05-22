# Persian G2P Tools Benchmark

This repository contains benchmarking notebooks for various Persian grapheme-to-phoneme (G2P) models, including both baseline models and the proposed Homo-GE2PE and Homo-T5 models in the *[Fast, Not Fancy: Rethinking G2P with Rich Data and Rule-Based Models]([link](https://arxiv.org/abs/2505.12973))* study. The benchmarks are conducted using the [SentenceBench Persian G2P Benchmark](https://huggingface.co/datasets/MahtaFetrat/SentenceBench).

---

## Repository Structure

```
benchmarking-scripts/
│   ├── Benchmark_AzamRabiee_Persian_G2P.ipynb
│   ├── Benchmark_GE2PE.ipynb
│   ├── Benchmark_HomoFast_eSpeak.ipynb
│   ├── Benchmark_Homo_GE2PE.ipynb
│   ├── Benchmark_Homo_T5.ipynb
│   ├── Benchmark_PasaOpasen_PersianG2P.ipynb
│   ├── Benchmark_de_mh_persian_phonemizer.ipynb
│   ├── Benchmark_dmort27_epitran.ipynb
│   ├── Benchmark_eSpeak_NG.ipynb
│   └── Benchmark_mohamad_hasan_sohan_ajini_G2P.ipynb
│   └── Benchmark_sajadalipour7_Persian_Grapheme_To_Phoneme_With_Transformer.ipynb
```

Each notebook benchmarks a specific model using the SentenceBench dataset. The results of each run (5 independent runs per model) are documented in the last markdown cell of each notebook.

---

### Benchmarking Results

The table below presents the performance of each model, averaged across 5 runs:

| Model                                                                                                           | PER (%) | Homograph Acc. (%) | Avg. Inf. Time (s) |
| ----------------------------------------------                                                                  | ------- | ------------------ | ------------------ |
| [Persian\_G2P](https://github.com/AzamRabiee/Persian_G2P)                                                       | 35.23   | 21.23              | 11.1374            |
| [PersianG2P](https://github.com/PasaOpasen/PersianG2P)                                                          | 15.04   | 37.74              | 2.1686             |
| [persian\_phonemizer](https://github.com/de-mh/persian_phonemizer)                                              | 25.27   | 29.25              | 0.1803             |
| [Epitran](https://github.com/dmort27/epitran)                                                                   | 45.12   | 0.00               | 0.0003             |
| [Persian G2P](https://github.com/mohamad-hasan-sohan-ajini/G2P)                                                 | 19.63   | 29.91              | 28.0039            |
| [Persian\_Grapheme\_To\_Phoneme](https://github.com/sajadalipour7/Persian-Grapheme-To-Phoneme-With-Transformer) | 12.85   | 40.00              | 0.9685             |
| [eSpeak NG](https://espeak.sourceforge.net/)                                                                    | 6.92    | 43.87              | 0.0169             |
| [GE2PE](https://github.com/Sharif-SLPL/GE2PE)                                                                   | 4.81    | 47.17              | 0.4464             |
| [HomoFast eSpeak](https://github.com/MahtaFetrat/HomoFast-eSpeak-Persian)                                       | 6.33    | 74.53              | 0.0084             |
| [Homo-T5](https://github.com/MahtaFetrat/Homo-GE2PE-Persian)                                                    | 4.12    | 76.32              | 0.4141             |
| [Homo-GE2PE](https://github.com/MahtaFetrat/Homo-GE2PE-Persian)                                                 | 3.98    | 76.89              | 0.4473             |

---

## Contributions

Contributions and pull requests are welcome. Please open an issue to discuss the changes you intend to make or the models/ttols you want to add to the benchmark.

---

### Additional Links

* [Link to Paper](https://arxiv.org/abs/2505.12973)
* [SentenceBench Persian G2P Benchmark](https://huggingface.co/datasets/MahtaFetrat/SentenceBench)
