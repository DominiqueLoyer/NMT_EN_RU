# Neural Machine Translation System: English-to-Russian

Complete implementation of English-to-Russian neural machine translation system using attention mechanisms and transformer architectures.

## Overview

This project develops and evaluates a neural machine translation (NMT) system for English-to-Russian translation using modern deep learning approaches. The system fine-tunes the Helsinki-NLP/opus-mt-en-ru pre-trained model on the opusbooks dataset.

## Features

- Transformer-based architecture with attention mechanisms
- Fine-tuned Helsinki-NLP/opus-mt-en-ru model
- Training on 10,000+ sentence pairs from opusbooks
- Evaluation using multiple metrics (BLEU, chrF, TER)
- Handling of Russian morphological complexity
- Integration with Hugging Face Transformers library

## Performance Metrics

- **SacreBLEU Score:** 22.6
- **chrF Score:** 48.5
- **Training:** Kaggle T4 GPU environment
- **Dataset:** OpenParallel opusbooks (EN-RU)

## Installation

```bash
pip install torch transformers datasets evaluate
```

## Hugging Face Model Card

See: https://huggingface.co/Helsinki-NLP/opus-mt-en-ru

## License

MIT License - See LICENSE file for details

## Author

**Dominique S. Loyer**
- ORCID: https://orcid.org/0009-0003-9713-7109
- GitHub: https://github.com/DominiqueLoyer
- Affiliation: Universite du Quebec a Montreal (UQAM)

## Challenges & Solutions

### Russian Morphological Complexity
- Solution: Fine-tuning on morphologically rich dataset
- Pre-trained model handles inflectional suffixes
- Subword tokenization captures Russian morphology

### Data Quality
- Solution: Filtering of low-quality alignments
- Validation on in-domain test set
- Manual review of translation outputs

## Future Work

- [ ] Multilingual support (French, German)
- [ ] Bidirectional translation (RU-EN)
- [ ] Domain-specific fine-tuning
- [ ] Integration with back-translation for data augmentation
- [ ] Evaluation on news domain benchmark

## Contributing

Contributions welcome! Areas of interest:
- Back-translation data augmentation
- Domain adaptation experiments
- Evaluation on standard benchmarks

---

**Last Updated:** January 6, 2026
**Status:** Ready for production use
