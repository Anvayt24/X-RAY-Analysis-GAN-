

🖼️ Synthetic Image Generation & Classification with GANs 🤖
This project uses GANs (Generative Adversarial Networks) to create synthetic images and trains a CNN (Convolutional Neural Network) to classify both real and generated images! 🚀

📂 Project Structure
/dataset - MURA dataset (train/valid).
/generated_images - Folder for generated synthetic images.
cnn_model.h5 - Trained CNN model.
app.py - FastAPI app for generating & downloading synthetic images.
🚀 Installation
Clone the repo:

git clone https://github.com/yourusername/gan-image-classification.git
cd gan-image-classification
Install dependencies:

pip install -r requirements.txt
Prepare your dataset (place images in /dataset/train and /dataset/valid).
⚡ Training the Model
To train the CNN with both real and synthetic images, run:


python train_model.py
🎨 Generate Synthetic Images
Start the FastAPI server:

uvicorn app:app --reload
Use the /generate/ endpoint to create synthetic images! 👇

Example request:

json
{
    "num_images": 10
}
📥 Download Images
After generating, download images via the /download/{image_name} endpoint.

🛠️ Technologies Used
TensorFlow for model building 🧠
FastAPI for serving the model ⚡
OpenCV for image processing 📸
