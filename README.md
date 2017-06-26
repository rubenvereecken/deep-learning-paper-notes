# Deep Learning Paper Notes

This repository is a collaborative effort to summarize and help interpret research papers vaguely related to deep learning. Inspired by [dennybritz/deeplearning-papernotes](https://github.com/dennybritz/deeplearning-papernotes).

Papers are subdivided into entirely arbitrary categories.

## Tooling

There are some tools to help you get started so you can dig in right away. You will need `node` and `npm` to use them. Install using:

`npm install -g https://github.com/rubenvereecken/paper-notes-tools.git`

This will install the executable `add-paper`, which currently just works for arXiv URLs. Use it like:

`add-paper https://arxiv.org/abs/1704.00784 --category=attention`

It will then add an entry to the `README.md` and a new file under the designated category.

## Papers

### Attention

#### 2017

*   [x] Online and Linear-Time Attention by Enforcing Monotonic Alignments [[notes](attention/2017-raffel-online_and_linear_time_attention_by_enforcing_monotonic_alignments.md)] [[arXiv](https://arxiv.org/abs/1704.00784)]
*   [ ] Attention Is All You Need [[notes](attention/2017-vaswani-attention_is_all_you_need.md)] [[arXiv](https://arxiv.org/abs/1706.03762)]

#### 2016

*   [x] Lip Reading Sentences in the Wild [[notes](attention/2016-chung-lip_reading_sentences_in_the_wild.md)] [[arXiv](https://arxiv.org/abs/1611.05358)]

#### 2015

*   [x] Show, Attend and Tell: Neural Image Caption Generation with Visual Attention [[notes](attention/2015-xu-show_attend_and_tell_neural_image_caption_generation_with_visual_attention.md)] [[arXiv](https://arxiv.org/abs/1502.03044)]
*   [ ] Describing Multimedia Content using Attention-based Encoder-Decoder Networks [[notes](attention/2015-cho-describing_multimedia_content_using_attention_based_encoder_decoder_networks.md)] [[arXiv](https://arxiv.org/abs/1507.01053)]
*   [x] Effective Approaches to Attention-based Neural Machine Translation [[notes](attention/2015-luong-effective_approaches_to_attention_based_neural_machine_translation.md)] [[arXiv](https://arxiv.org/abs/1508.04025)]
*   [x] Attention-Based Models for Speech Recognition [[notes](attention/2015-chorowski-attention_based_models_for_speech_recognition.md)] [[arXiv](https://arxiv.org/abs/1506.07503)]

#### 2014

*   [x] Neural Machine Translation by Jointly Learning to Align and Translate [[notes](attention/2014-bahdanau-neural_machine_translation_by_jointly_learning_to_align_and_translate.md)] [[arXiv](https://arxiv.org/abs/1409.0473)]

### Neural Networks

#### 2016

*   [x] On the Expressive Power of Deep Neural Networks [[notes](neural-networks/2016-raghu-on_the_expressive_power_of_deep_neural_networks.md)] [[arXiv](https://arxiv.org/abs/1606.05336)]

## Related Efforts

*   [dennybritz/deeplearning-papernotes](https://github.com/dennybritz/deeplearning-papernotes)

## Contributing

Anything goes. Have a look at how existing notes are written

### Formatting

I like [semantic linefeeds](http://rhodesmill.org/brandon/2012/one-sentence-per-line/). Give it a skim and be convinced.
