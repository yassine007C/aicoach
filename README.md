# aicoach
🚀 Getting Started
1. Clone or open the notebook
Open the aico.ipynb notebook on Google Colab.

2. Install dependencies
python
Copier
Modifier
!pip install --upgrade google-generativeai ultralytics opencv-python-headless
3. Upload your video
The notebook will prompt you to upload a .mp4 or .avi football match video.

python
Copier
Modifier
from google.colab import files
uploaded = files.upload()
4. Run the analysis
python
Copier
Modifier
analyze_video_every_30s(video_path, interval_sec=30)
🔐 API Key
This project uses Google Gemini API for generating tactical insights. Set up your key like this:

python
Copier
Modifier
genai.configure(api_key="YOUR_GEMINI_API_KEY")
💡 Note: Never share your API key in public repositories. Use environment variables or Colab secrets for security.

🧠 Tactical Analysis Example
"Our team is playing a 4-3-3 formation with 11 players detected. The ball is detected.
Provide a brief tactical insight."

Gemini Insight:

"The 4-3-3 formation provides strong wing play. Consider switching to a 4-2-3-1 if midfield pressure increases."
