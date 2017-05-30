# Online and Linear-Time Attention by Enforcing Monotonic Alignments

https://arxiv.org/abs/1704.00784


## Notes
- Attention mechanism with linear-time complexity (at inference, not training) that works in online settings for monotonic seq2seq
- Instead of aligning to any input, only forward jumps are allowed from the last selected input. Strong assumption of monotonicity
- Based on sampling but uses expected contect to make it learnable through backpropagation. Then at inference time they use hard attention that has the same effect as learned during training even though it’s entirely different. It’s clever. Quite a few small tricks to make this work though
- Interesting rescaling of the energy term as they use the sigmoid (still not 100% sure why) and it’s supposedly sensitive to that. Tensorflow now supports this rescaling in their attention implementation thanks to this paper

## Implementation
- https://github.com/craffel/mad


## Thoughts
- Very good "related work" section
