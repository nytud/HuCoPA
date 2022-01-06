# HuCoPA
This is the home repository for the Hungarian Choice of Plausible Alternatives Corpus (HuCoPA), which is also part of the Hungarian Language Understanding Evaluation Benchmark Kit [HuLU](hulu.nlp.nytud.hu). The corpus was created by translating and re-annotating the original English CoPA corpus. 

## License and usage

The corpus is available under the license CC-BY-SA 4.0. If you use this corpus, please cite our paper, and the original CoPA corpus' paper (see below). 

## Data

The files are in the 'data' folder. The dataset contains 1 000 instances. Each instance is composed of a premise and two alternatives. The task is to select the alternative that describes a situation standing in causal relation to the situation described by the premise.

The train, devel and test sets contain 400, 100 and 500 instances, respectively, following the splits of the original English dataset (as in the GLUE benchmark). The test set is distributed without the labels; to evaluate your model please contact us (ligeti-nagy.noemi@nytud.hu) or visit [HuLU's website](hulu.nlp.nytud.hu) for an automatic evaluation (under construction). 

## Data format

The data files are in json format. The keys are the following:

`idx`: unique id of the instances, an integer between 1 and 1000;

`question`: "cause" or "effect". It suggests what kind of causal relation are we looking for: in the case of "cause" we search for the more plausible alternative that may be a cause of the premise. In the case of "effect" we are looking for a plausible result of the premise;

`premise`: the premise, a sentence; 

`choice1`: the first alternative, a sentence; 

`choice2`: the second alternative, a sentence;

`label`: the number of the more plausible alternative (1 or 2).

## Guidelines

Later...

## Citation

If you use this resource or any part of its documentation, please refer to:

Later...


and to:

Roemmele, M., Bejan, C., and Gordon, A. (2011) Choice of Plausible Alternatives: An Evaluation of Commonsense Causal Reasoning. AAAI Spring Symposium on Logical Formalizations of Commonsense Reasoning, Stanford University, March 21-23, 2011.
```
@inproceedings{roemmele2011choice,
  title={Choice of plausible alternatives: An evaluation of commonsense causal reasoning},
  author={Roemmele, Melissa and Bejan, Cosmin Adrian and Gordon, Andrew S},
  booktitle={2011 AAAI Spring Symposium Series},
  year={2011},
  url={https://people.ict.usc.edu/~gordon/publications/AAAI-SPRING11A.PDF},
}
```
