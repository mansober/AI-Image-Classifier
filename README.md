Markdown
# AI Image Classifier

A lightweight web application built to explore how pre-trained deep learning models can be integrated into interactive web interfaces. This project takes user-uploaded images and classifies them using TensorFlow's MobileNetV2.

##  Project Goals & What I Learned
I built this project to gain hands-on experience with computer vision and machine learning deployment. Through this build, I learned how to:
* Process and format image data using **NumPy** and **OpenCV** so it can be read by a neural network.
* Implement a pre-trained deep learning model (**MobileNetV2**) rather than building one from scratch.
* Create a clean, interactive frontend rapidly using **Streamlit**.
* Manage environments and optimize performance using model caching (`@st.cache_resource`).

##  How It Works
* **Upload:** Users can upload any `.jpg` or `.png` image.
* **Analyze:** The image is resized and preprocessed to fit the model's required input format.
* **Predict:** The AI evaluates the image and returns the top 3 most likely classifications along with confidence percentages.

##  Tech Stack
* **Language:** Python
* **Frontend:** Streamlit
* **Machine Learning:** TensorFlow / Keras
* **Image Processing:** OpenCV (`opencv-python-headless`), NumPy, Pillow
* **Environment:** `uv`

##  How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/mansober/AI-Image-Classifier](https://github.com/mansober/AI-Image-Classifier)
   cd your-repo-name
Install dependencies:
(Ensure you have uv installed)

2. **Install dependencies:**
   *(Ensure you have uv installed)*
   ```bash
   uv pip install -r requirements.txt
   ```

3. **Run the application:**
   ```bash
   uv run streamlit run main.py
   ```
