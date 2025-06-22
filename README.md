# VAE on CelebA Dataset

In this project, we compare deep generative models: **Variational Autoencoder (VAE)** using the CelebA dataset. We aim to evaluate its ability to generate realistic human face images and understand their strengths and limitations.

**Dataset source**: [CelebFaces Attributes Dataset (CelebA)](https://www.kaggle.com/datasets/jessicali9530/celeba-dataset)


## Final Report Conclusion

In this project, we successfully implemented and trained a **Variational Autoencoder (VAE)** on the CelebA face dataset. Our pipeline included the following stages:

1. **Model Construction**  
   - Designed and implemented a custom VAE architecture using TensorFlow and Keras.
   - Defined the encoder, decoder, and VAE model class with custom training logic that computes both **reconstruction loss** and **KL divergence**.

2. **Model Training**  
   - Trained the VAE for 10 epochs using the CelebA dataset.
   - Monitored losses during training, observing a steady decline in both total loss and reconstruction loss, while the KL divergence remained stable.
   - The learning process appeared stable and effective for the given number of epochs.

3. **Qualitative Evaluation**  
   - Visualized reconstruction results showing that the VAE successfully captures facial structure and reconstructs input images with reasonable fidelity.
   - Sampled new faces from the latent space, verifying the generative capability of the model.
   - Performed **latent space interpolation**, which showed smooth semantic transitions between faces, indicating a well-structured latent space.

4. **Loss Analysis**  
   - Plotted total loss, reconstruction loss, and KL loss across epochs.
   - Observed that the total loss is dominated by reconstruction error, while the KL term contributes a small but consistent regularization effect.

### Conclusion
The VAE demonstrates solid reconstruction and generative performance on the CelebA dataset, even with only 10 training epochs. The loss trends suggest the model is effectively learning both pixel-level fidelity and latent structure regularization. With extended training or hyperparameter tuning (e.g., KL annealing or β-VAE), further improvements could be expected. The project confirms VAE’s ability to model complex image distributions and opens doors to potential applications in image generation, compression, and style transfer.

---



