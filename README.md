# Smol-GPT

A lightweight, decoder-only Transformer (GPT-like) language model built entirely from scratch using PyTorch.

This project demonstrates the core building blocks of GPT models such as:

- Multi-head self-attention
- Feedforward neural networks
- Layer normalization
- Positional embeddings
- Causal masking for autoregressive token generation

---

## 🧠 Model Architecture

- Decoder-only Transformer
- Multi-head Self-Attention
- Stack of `n_layer` Transformer blocks
- Character-level language modeling

---

## 📁 Project Structure

```
.
├── input.txt              # Training corpus (e.g. Shakespeare, song lyrics, etc.)
├── final_gpt.py          # Final model and training logic
└── README.md             # Project documentation
```

---

## 🚀 How to Run

1. **Clone the repo**:

```bash
git clone https://github.com/Zaheerkhn/Smol-GPT
```

2. **Add your training text** to `input.txt`:

> Example: paste Shakespeare text, song lyrics, or any large plain-text file.

3. **Run the training script**:

```bash
python final_gpt.py
```

The model will:

- Train on the given text
- Print training and validation loss every few steps
- Generate a sample of text after training

---

## ⚙️ Hyperparameters

All key parameters can be modified at the top of the script:

| Parameter       | Value | Description                           |
| --------------- | ----- | ------------------------------------- |
| `n_embd`        | 384   | Embedding dimension                   |
| `n_head`        | 6     | Number of attention heads             |
| `n_layer`       | 6     | Number of transformer blocks          |
| `block_size`    | 256   | Max sequence length for training      |
| `batch_size`    | 64    | Number of sequences per training step |
| `learning_rate` | 3e-4  | AdamW optimizer learning rate         |
| `dropout`       | 0.2   | Dropout rate for regularization       |
| `max_iters`     | 5000  | Number of training iterations         |

---

## 📌 Sample Output

After training, the model will generate text like this:

```
and the king did speaketh
with tongue of fire and flame,
the lands did tremble on his name.
```

> Output quality improves with more data and training time.

---

## 🧪 Training Data

Use any `.txt` file as training data. Some fun ideas:

- Shakespeare plays
- Wikipedia articles
- Your chat logs
- Famous speeches
- Song lyrics

Just replace `input.txt` with your desired dataset.

---

## 📜 License

This project is licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

---

## 🙌 Acknowledgements

Inspired by:

- [Andrej Karpathy’s nanoGPT](https://github.com/karpathy/nanoGPT)

---

