# SMARTDERM-AI-POWERED-SKIN-DISEASE-DETECTION-AND-TREATMENT-SUGGESTION
An AI-based system using MobileNetV2 to detect skin diseases like Acne, Eczema, and Psoriasis from images with ~80% accuracy. Built with Flask and HTML/CSS, it provides instant diagnosis and treatment suggestions, offering a user-friendly, accessible solution for early skin health assessment, especially in underserved regions.

Steps to Run the Skin Disease Detection Project on Your PC: 
1. Open Command Prompt & Navigate to Project Folder 
cd "C:\Users\YourUsername\Desktop\Skin Disease Project"  
2. Create & Activate Virtual Environment (Recommended)  
(A) Create Virtual Environment python -m venv venv  
(B) Activate Virtual Environment  
• Windows:   
• venv\Scripts\activate  
• Linux/Mac:   
• source venv/bin/activate  
3. Install Required Dependencies 
pip install -r requirements.txt  
If requirements.txt is missing, install manually:  
pip install flask tensorflow keras numpy opencv-python pillow  
4.  Ensure Model & Necessary Folders Exist Check 
for:  
• model.h5 (trained model)  
• static/ (for CSS, JS, images)  
• uploads/ (for uploaded images)  
• templates/ (for HTML) If missing:  
mkdir static uploads  
5. Run the Flask App python 
app.py  
If successful, you will see:  
Running on http://127.0.0.1:5000/  
Open http://127.0.0.1:5000/ in your browser.  
6. Troubleshooting (A) If 
Port is Busy python 
app.py --port 5001  
Access it at: http://127.0.0.1:5001/  
(B) If FileNotFoundError  
Ensure uploads/ and static/ exist: mkdir 
uploads static  
(C) Running on Local Network  
1. Find Local IP:   
2. ipconfig (Windows) OR ifconfig (Linux/Mac)  
3. Run Flask with:   
4. python app.py --host=0.0.0.0 --port=5000 5. Open 
from any device on the same Wi-Fi:   
6. http://<Your_Local_IP>:5000  
Now Your Project is Running on Your PC!    
