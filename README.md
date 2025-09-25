EduHub Schools Website
A modern, dynamic website for Primary and Secondary schools, built with React and Tailwind CSS, featuring a virtual tour, role-based access, and Faculty/Student Portal pages.
Features

Responsive Design: Mobile-friendly with hamburger menu (≤640px).
Header: Minimalist, centered logo (“EduHub Schools”, 1.25rem), single-line nav (Welcome, Programs, Admissions, Events, Faculty, Portal, Contact, 0.9rem), small avatar dropdown (Light/Dark/Primary/Secondary, language, login).
Footer: Matches header style (white background, centered logo 1.25rem, social icons, copyright, Navy Blue #1E3A8A text, z-index: 50), no nav links to reduce redundancy.
Welcome: Text-only section with title, writeup: “EduHub Schools empowers students through dynamic primary and secondary education, nurturing innovation and collaboration,” and CTA to Programs.
Homepage: Single-column news cards with school-themed images.
Programs: Expandable cards for Primary (e.g., “Math Quest”) and Secondary (e.g., “Biology Adventures”) with icons (star/book), solid white card background (#FFFFFF) like Events, Navy Blue #1E3A8A dropdown text and titles, Charcoal Gray #374151 descriptions.
Admissions: Centered form with admissions guide download button.
Events: Single-column event cards with date badges, solid white background (#FFFFFF).
Faculty: Faculty cards with school-themed profile images.
Student Portal: Role-based content (schedules, resources) or login prompt.
Contact/Map: Clean map above contact form.
Virtual Tour: 360-degree viewer with Pannellum.
Role-Based Access: Mock JWT login (student, faculty, admin).
Notifications: Dismissible event alerts.
Themes: Light (Mint Green #E6FFFA background, Navy #1E3A8A primary), Dark (Dark Slate #1F2937 background, Light Navy #3B82F6 primary), Primary (Navy-heavy, rounded), Secondary (Yellow-heavy, sharp).
Multilingual: English, Spanish, French with i18next.
Analytics: Mock Google Analytics.
Design: Montserrat (headings) and Lato (body) fonts, Deep Navy Blue (#1E3A8A), Warm Yellow (#FBBF24), Soft Mint Green (#E6FFFA) background with colorful book/pencil pattern (20px, 0.05 opacity), flat cards, slide-up animations, hover-scale buttons.
Error Handling: Error boundaries and image fallbacks.
Text Visibility: All text (sections, footer) uses high-contrast colors (#1E3A8A, #374151, #FFFFFF, z-index: 50).

Setup

Save index.html, styles.css, README.md in C:\Users\USER\schoolwebsite.

Install http-server:
npm install -g http-server


Run server:
cd C:\Users\USER\schoolwebsite
http-server


Open http://127.0.0.1:8080 in Chrome.


Deployment

GitHub Pages:
Initialize Git:
cd C:\Users\USER\schoolwebsite
git init
git add .
git commit -m "Commit Message"
git remote add origin https://github.com/your-username/school-website.git
git push -u origin main


In GitHub, Settings > Pages, select main branch, / (root).

Visit https://your-username.github.io/school-website.



Netlify: Drag and drop schoolwebsite folder or connect GitHub repo at netlify.com.

Testing

Open http://127.0.0.1:8080 in Chrome (12:46 PM WAT, Sep 25, 2025).
Test responsiveness with Chrome DevTools (mobile, tablet, desktop).
Check DevTools > Console for errors.
Clear cache or use Incognito mode (Ctrl+Shift+N).
Verify:
Programs: Expandable cards show Primary (“Math Quest”, “Science Explorers”), Secondary (“Biology Adventures”, “Creative Writing”), and test card (“Test Course”) with solid white card background (#FFFFFF), Navy Blue #1E3A8A dropdown text and titles, Charcoal Gray #374151 descriptions, z-index: 50.
Theme Toggle: Avatar dropdown shows Light/Dark/Primary/Secondary options at the top, switches themes (Light: #E6FFFA, Dark: #1F2937).
Footer: White background, centered logo (1.25rem), social icons, copyright, Navy Blue #1E3A8A text, z-index: 50, no nav links.
Background: Soft Mint Green (#E6FFFA) with book/pencil pattern (20px, 0.05 opacity).
Header: Centered logo (1.25rem), single-line nav (0.9rem), avatar dropdown.
Homepage: News cards with school images.
Admissions: Centered form, download button.
Events: Cards with badges, solid white background (#FFFFFF).
Faculty: Cards with school-themed images.
Student Portal: Role-based content or login.
Contact/Map: Map above form.
Virtual Tour: Pannellum viewer.
Design: Navy (#1E3A8A), Yellow (#FBBF24), Mint Green (#E6FFFA), Montserrat/Lato, slide-up animations.
Spacing: 1.25rem section padding, gap-2.5 for cards.
Images: School-themed (picsum.photos, e.g., ?random=30) or “Image Unavailable”.
No blank page: Error boundaries display fallback.



Troubleshooting

Programs Text Not Visible: Check DevTools > Elements for .program-content (background-color: #FFFFFF). Verify .program-button has color: #1E3A8A. Log store.getState().programs in Console. Confirm toggleCard and openCard state.

Theme Toggle Not Showing: Inspect .theme-select in DevTools for display: block, visibility: visible, z-index: 60. Log isDropdownOpen in Console. Clear cache (Ctrl+Shift+R) or use Incognito (Ctrl+Shift+N).

Footer Content: Verify .footer has background-color: #FFFFFF, color: #1E3A8A, no .nav, only logo, social icons, and copyright.

CDN Errors: Check internet (ping cdn.jsdelivr.net). Use local dependencies:
npm install leaflet react-leaflet pannellum i18next react-i18next

Copy to schoolwebsite/lib/ and update <script> tags.

Blank Page: Check DevTools > Console. Ensure CDNs load (status 200). Refresh or clear cache.


Notes

Replace picsum.photos with real school images.
Add backend (e.g., Firebase) for notifications and forms in production.
Update README.md “Demo” with deployed URL.
Resume Pitch: "Developed a dynamic school website with React, featuring solid white card backgrounds for Programs section, visible light/dark mode toggle, and optimized UI, showcasing expertise in responsive design and debugging."

Demo
[Insert deployed URL after deployment]