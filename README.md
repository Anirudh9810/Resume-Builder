Theme Flexibility & Expanded Resume Details Plan
Upgrade the AI Resume Tailor to be theme-aware and collect richer professional data for more comprehensive tailoring.

Proposed Changes
[MODIFY] 
index.html
1. Adaptive Theming
CSS Variables: Refactor :root to support two themes (Dark/Light).
System Detection: Use (prefers-color-scheme: dark) media query for initial load.
Manual Toggle: Add a "Sun/Moon" button in the header to switch themes.
Persistence: Save the user's theme preference in localStorage.
2. Expanded Resume Form (Step 2)
Education Section:
Implement a dynamic list similar to "Experience".
Fields: Degree, Institution, Year/Duration.
Additional Sections:
Languages: A text area to capture linguistic proficiencies.
Interests/Hobbies: A section for extra-curricular activities.
Strengthen Info: A dedicated "Additional Context" field for users to provide extra background that the AI should use to boost the resume.
3. AI Logic Updates
Parsing Prompt: Update the extraction logic to attempt finding Education, Languages, and Hobbies in uploaded files.
Generation Prompt: Update the tailor engine to incorporate:
Educational background as a separate section.
Languages and Hobbies as footer/sidebar elements (as appropriate for a professional resume).
"Additional Context" as a high-weight factor for tailoring bullet points.
User Review Required
IMPORTANT

The AI will now have more data to process. This might slightly increase generation time but will lead to a much more "human-like" and tailored output.

Verification Plan
Manual Verification
Test theme switching (Light/Dark) and verify system preference detection.
Verify that new fields (Education, etc.) are correctly saved to the internal state.
Test PDF/DOCX upload to see if Gemini successfully extracts Education details.
Generate a resume and check if the new sections (Education, Languages) appear in the output.
