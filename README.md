# 🚀 Transformers from Scratch: Building the Encoder, Step-by-Step!

**📜 Based on the legendary paper:** [Attention Is All You Need (Vaswani et al., 2017)](https://arxiv.org/abs/1706.03762)

Hey! 👋

Ever felt that Transformers were some kind of black magic? Heard "Attention Is All You Need" but got a bit lost trying to connect the dots from paper to actual, runnable code? You're definitely not alone, and you've come to the right place!

This repository is your **super-friendly, hands-on guide** to building the **Transformer Encoder** from the ground up using **PyTorch**. We're not just talking theory here; we'll go **module by module, line by line (almost!)**, breaking down all the "scary" stuff into simple, understandable pieces.

My goal? To help you *really get* how these things tick.

---

## 🎯 What's the Real Goal Here?

This isn't just about copying some code. It's about empowering you to:

-   🛠️ **Build your own Transformer Encoder** from scratch and *understand every part*.
-   🧠 Get a solid intuition for **self-attention, multi-head attention, positional encoding**, and all those other cool concepts.
-   📖 Read modern NLP papers with more confidence because you've seen the mechanics firsthand.
-   🧪 Lay the groundwork to **tackle more complex models** later (like building Decoders for GPT-style models, or understanding BERT).
-   🚀 Feel that awesome "Aha!" moment when it all clicks.

---

## 💡 Where to Find the Full Tutorial Experience?

While this repo contains all the code, the **best way to learn** is by following the interactive notebook:

*   ➡️ **Interactive Notebook:** [`main.ipynb`](./main.ipynb) (This is where the magic happens!)
*   **(Optional: Add links if you publish elsewhere)**
    *   📝 **Read it on Medium:** [Link to your Medium article]
    *   💻 **Run it on Kaggle:** [Link to your Kaggle Notebook]

---

## 🧱 What You'll Actually Build & Understand (Encoder Edition!)

We're focusing on the **Encoder** part of the Transformer architecture. Here's a sneak peek of the concepts we'll demystify and implement:

*   **Token Embeddings:** Turning words into numbers the model can understand.
*   **Positional Encoding:** Giving the model a sense of word order (super important since Transformers process words all at once!). We'll implement a learnable version.
*   **Self-Attention Mechanism:**
    *   The famous **Query, Key, and Value** vectors.
    *   **Scaled Dot-Product Attention:** The core math, but we'll make it feel simple.
*   **Multi-Head Attention:** Why having multiple "perspectives" (attention heads) helps the model learn richer representations.
*   **Feed-Forward Networks (within the Transformer block):** The other essential computational unit.
*   **Residual Connections & Layer Normalization:** The unsung heroes that make deep networks trainable. We'll be using the **Pre-LN** (LayerNorm before) variant.
*   **Putting it all together:**
    *   `SingleAttentionHead`
    *   `MultiHeadAttention`
    *   `TransformerBlock`
    *   And finally, the complete `Encoder` module by stacking these blocks.

---

## 🧠 Architecture We're Building (The Encoder)

This is the beast we're taming, one piece at a time:

<img src="encoder_architecture.png" alt="Transformer Encoder Architecture" width="400"/>

> 📌 Looks a bit much? Don't sweat it! The whole point of this repo is to show you it's totally buildable, step-by-step.

---

## 🔧 Get It Running

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/nls-forev/transformer-from-scratch.git
    cd transformer-from-scratch
    ```

2.  **Set up a Virtual Environment (Recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  **Install Dependencies:**
    We mostly need PyTorch. A `requirements.txt` is also provided.
    ```bash
    pip install torch torchvision torchaudio
    # Or, if you have the requirements.txt:
    # pip install -r requirements.txt
    ```
    *(Make sure you install the PyTorch version compatible with your CUDA if you plan to use a GPU, though this project runs fine on CPU).*

---

## 🚀 Let's Get Coding!

Once you've got everything set up:

1.  Open the `main.ipynb` notebook in Jupyter Lab, Jupyter Notebook, VS Code, or your favorite environment.
2.  Follow along, run the cells, experiment, and see the Transformer Encoder come to life!

---

## 🔮 What's Next? (Stay Tuned!)

This encoder is a powerful building block! In future tutorials (linked here when ready), we'll explore:

*   Using this encoder for tasks like **IMDb sentiment analysis**.
*   Building the **Decoder** part to create **GPT-style language models**.

---

## 🙏 Acknowledgements

*   The original "Attention Is All You Need" paper by Vaswani et al. for laying the foundation.
*   Countless explanations and tutorials from the community that have helped shape understanding.

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

Happy building! If you find this useful, a ⭐ on the repo would be much appreciated!