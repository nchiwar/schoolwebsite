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


Open http://127.0.0.1:8080



Notes

Replace picsum.photos with real school images.
Add backend (e.g., Firebase) for notifications and forms in production.
Update README.md “Demo” with deployed URL.
Resume Pitch: "Developed a dynamic school website with React, featuring solid white card backgrounds for Programs section, visible light/dark mode toggle, and optimized UI, showcasing expertise in responsive design and debugging."

Demo
https://nchiwar.github.io/schoolwebsite/

