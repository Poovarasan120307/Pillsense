PILLSENSE - AI Prescription Explainer for Elderly Patients
REVA University | Introduction to Design Thinking

WHAT IS IN THIS FOLDER
  index.html   The complete website (HTML, CSS and JavaScript in one file)
  README.txt   This file

HOW TO RUN ON A LAPTOP
  Option A: double-click index.html (opens in Chrome).
  Option B (recommended): open a terminal in this folder and run
      python -m http.server 8000
  then open http://localhost:8000 in Chrome.
  The camera works on localhost.

HOW TO USE ON A PHONE (camera needs https)
  1. Go to https://app.netlify.com/drop
  2. Drag this whole folder onto the page.
  3. Open the https link it gives you on your phone.

FIRST-TIME SETUP
  1. Get a free Gemini API key at https://aistudio.google.com/app/apikey
  2. Open the site, expand "Settings", paste the key.
  3. If you see "model not found", type another current Gemini Flash
     model name in the Model box (default: gemini-2.5-flash).

HOW TO DEMO
  1. Choose a language.
  2. Tap "Scan prescription", open the camera, take the photo, "Use this photo".
  3. You get the day plan (morning / afternoon / night) and explanations.
  4. Tap "Scan tablet cover" and scan each strip or box. The app reads the
     PRINTED name and strength and reports: matches your prescription,
     not on your prescription, strength different, or could not read.
  5. "Try the offline sample" shows a fixed example if the internet fails.
     It is labelled as a sample on screen.

SAFETY DESIGN (mention in your viva)
  - Tablets are identified only from printed text, never from colour,
    shape or size, because that is unreliable and unsafe.
  - Unclear text is flagged for retake instead of guessed.
  - A disclaimer is shown after every result: not medical advice,
    confirm with your doctor or pharmacist.
  - Photos are kept in memory only and are not stored.

NOTES
  - The API key is saved in your browser only. Do not share the site
    with your key saved in it. For a real deployment, put the key on a
    small server instead of in the browser.
  - Have a Kannada speaker check the Kannada text before presenting.
  - Test with sample prescriptions, not real patient details.
