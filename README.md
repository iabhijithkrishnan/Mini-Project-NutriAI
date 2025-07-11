NutriAI

Nutri AI is a mini web-based project designed to provide nutritional insights from food images using Artificial Intelligence. By leveraging machine learning and computer vision, it detects food items and estimates their nutritional values—such as calories, protein, carbohydrates, and fat.
This project showcases how AI technologies can enhance health and diet management.

Features
- Upload food images through a web interface
- Food recognition powered by YOLOv-based AI model
- Displays estimated nutritional information
- Frontend built with HTML, CSS, and JavaScript
- Backend implemented using Python (Flask)
- Modular and easy to extend for learning and experimentation

Tech Stack
- Frontend: HTML, CSS, JavaScript
- Backend: Python (Flask)
- AI Model: YOLO (You Only Look Once) — yolo11n.pt
- Libraries: OpenCV, Torch, Flask, PyYAML, NumPy
- Configuration: Custom model settings via yolo.yaml

Project Structure
Mini-Project-NutriAI/
│
├── frontend/           # Web interface files (HTML/CSS/JS)
├── routes/             # API route handlers (Flask)
├── app.py              # Main Flask backend
├── run_inference.py    # YOLO inference script
├── yolo.yaml           # Model configuration
├── yolo11n.pt          # Trained YOLO model
├── index.js            # Client-side logic
├── package.json        # JS dependencies
├── package-lock.json
└── README.md           # Project documentation



How to Run Locally
Prerequisites: Ensure Python and pip are installed. A virtual environment is recommended.

- Clone the repository
git clone https://github.com/iabhijithkrishnan/Mini-Project-NutriAI.git
cd Mini-Project-NutriAI


- Install Python dependencies
If a requirements.txt file is present:
pip install -r requirements.txt


If not, install manually:
pip install flask torch opencv-python pyyaml


- Run the Flask application
python app.py


- Access the web app
Open your browser and go to: http://localhost:5000

Notes
- The model file yolo11n.pt may be large and require Git LFS or alternative hosting
- Detection classes and configuration are customizable via yolo.yaml
- You can enhance the model by training on your own dataset

Future Enhancements
- Add user authentication and diet history tracking
- Enable real-time food recognition via webcam
- Improve recognition accuracy using larger models
- Integrate with fitness and health tracking APIs

