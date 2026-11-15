# Workshop 3 — How Neural Networks Learn

AIML-500 · Professional Portfolio Artifact 3

[Open the interactive demo](https://quiksun.github.io/AI-ML-Professional-Portfolio/Workshop3/training-methods.html) · [View the source file](./training-methods.html)

## Overview

This artifact combines **3.2 Neural Networks** with the **Professor Predict** opening activity from **3.3 AI Training Interaction**. The demo runs the same three prompts through four approaches so readers can compare how each one processes text, scores possible continuations, and uses feedback during training.

## Try the demo

1. Choose a prompt and select **Feedforward ANN**, **CNN**, **RNN**, or **GAN**.
2. Step through the walkthrough. In the CNN and RNN views, use the slider where available to inspect a word window or follow the hidden state one word at a time.
3. Select **Run one update** to compare the starting and updated probabilities. In the GAN view, select **Draw a sample** to see one word drawn from the generator’s distribution.

## The three prompts

| Prompt | What it demonstrates |
| --- | --- |
| “The capital of France is ___” | **Paris** shows how a familiar language pattern can produce a correct factual answer. |
| “Once upon a ___” | **time** shows how a common story opening shapes the next-word prediction. |
| “The current president of the small island nation of Velmora, founded in 1998, is ___” | **Velmora is fictional.** An invented name can still score highly. The unfamiliar country name and specific founding date prompted me to question the premise in the original exercise. |

## What each network learns from

| Approach | How it produces a continuation | Training feedback |
| --- | --- | --- |
| **Feedforward artificial neural network (ANN)** | Combines word cues using weights and a ReLU activation, then scores candidate words. | The next word in the training text supplies the target. |
| **Convolutional neural network (CNN)** | Slides each filter across three-word windows and uses its strongest response to score candidates. | The next word in the training text supplies the target. In full training, the prediction error can also guide updates to the filters. |
| **Recurrent neural network (RNN)** | Reads one word at a time, updates a hidden state, and uses the final state to score candidates. | The next-word target provides feedback on the prediction made from the sequence. |
| **Generative adversarial network (GAN)** | An RNN generator proposes a word. A CNN discriminator scores the completed phrase using patterns represented by its filters. | A discriminator score serves as a reward for the generator update. |

The ANN, CNN, and RNN examples use the same **self-supervised objective** because their target comes directly from the text. In **adversarial training**, the discriminator learns to distinguish training examples from generated ones, and its feedback guides the generator.

## Implementation and scope

The demo runs directly in a browser with JavaScript enabled. It uses hand-set starting weights and calculates probabilities over three candidate words per prompt. Each training step adjusts the output biases. The GAN exercise holds the discriminator fixed so readers can trace the effect of its feedback on the generator.

## References

- [IBM Developer, *A Beginner’s Guide to Artificial Intelligence and Machine Learning*](https://developer.ibm.com/articles/cc-beginner-guide-machine-learning-ai-cognitive/)
- [IBM, *What Is a Neural Network?*](https://www.ibm.com/think/topics/neural-networks) and [*What Is a Recurrent Neural Network?*](https://www.ibm.com/think/topics/recurrent-neural-networks)
- [Dauphin et al., *Language Modeling with Gated Convolutional Networks*](https://arxiv.org/abs/1612.08083)
- [IBM, *What Are Generative Adversarial Networks (GANs)?*](https://www.ibm.com/think/topics/generative-adversarial-networks)
- [Yu et al., *SeqGAN: Sequence Generative Adversarial Nets with Policy Gradient*](https://arxiv.org/abs/1609.05473)

## AI assistance

ChatGPT assisted with developing the interactive demo and drafting this documentation.
