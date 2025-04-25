. Download & Install Prerequisites
Visual Studio Code (VS Code)
Download Link: https://code.visualstudio.com/download

Installation: Run the downloaded installer (Windows/macOS/Linux).

Python
Download Link: https://www.python.org/downloads

Installation:

Check "Add Python to PATH" during installation.

Verify installation:

bash
python --version  # Should show Python 3.x
pip --version
2. Set Up a Virtual Environment (venv)
Create venv
Open VS Code and your project folder (diabetes-detection-website).

Open the VS Code terminal (Ctrl + `` `` or Terminal > New Terminal).

Run:

bash
python -m venv venv
This creates a venv folder in your project.

Activate venv
Windows:

bash
.\venv\Scripts\activate
macOS/Linux:

bash
source venv/bin/activate
You’ll see (venv) in the terminal prompt.

3. Install VS Code Extensions
Open the Extensions Marketplace (Ctrl+Shift+X).

Install these essential extensions:

Python (by Microsoft)

Pylance (for Python IntelliSense)

Jupyter (if using notebooks)

4. Install Dependencies
Ensure venv is active (check for (venv) in the terminal).

Install packages from requirements.txt:

bash
pip install -r requirements.txt
If requirements.txt is missing, manually install:

bash
pip install flask scikit-learn pandas numpy
5. Run the Diabetes Detection Website
Backend (Flask):

bash
python app.py
The terminal will show a local URL (e.g., http://127.0.0.1:5000).

Frontend:

Open index.html in a browser or navigate to the Flask server’s URL.

Troubleshooting
VS Code Python Interpreter:

Press Ctrl+Shift+P > "Python: Select Interpreter" > Choose the one from venv.

Missing Files: Ensure scaler.pkl, svm_model.pkl, and diabetes.csv are in the correct path (same folder as app.py).
