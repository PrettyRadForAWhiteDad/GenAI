# Dutch Shepherd: Intelligence, Versatility & Loyalty

**MBA Educational Website Project**

## Project Overview
A production-ready static educational website about Dutch Shepherd history, breed characteristics, temperament, training, care, responsible ownership, and lifestyle fit. The site is designed for GitHub Pages and uses only relative first-party paths.

## Features
- Multi-page responsive design
- Ask Dax client-side knowledge-base chatbot with 29 topics
- Dutch Shepherd suitability quiz
- Embedded educational YouTube video
- AI-generated working-dog video placeholder
- Breed and coat comparisons
- Responsive historical timeline and gallery
- Accessibility features and reduced-motion support
- Academic sources and GitHub Pages deployment support

## Technology
HTML5, CSS3, Vanilla JavaScript, sessionStorage, and GitHub Pages. No build process, API key, database, or backend is required.

## Project Structure
Root HTML files share `css/styles.css`, `js/chatbot-data.js`, `js/chatbot.js`, and `js/script.js`. First-party media belongs under `assets/images`, `assets/video`, and `assets/captions`. The empty `.nojekyll` file prevents Jekyll processing.

## Running Locally
Open `index.html` directly. Most features work when the file is opened directly; some browser security behaviors are more consistent through a simple static server, but a server is not a production requirement.

## GitHub Pages Deployment
1. Create a GitHub repository, suggested name `dutch-shepherd-mba`.
2. Add all files while preserving the folder structure.
3. Confirm `index.html` and `.nojekyll` are in the repository root.
4. Commit and push.
5. Open the repository on GitHub.
6. Navigate to **Settings → Pages**.
7. Select the appropriate publishing source in the current interface.
8. Publish from the intended branch and root folder.
9. Wait for deployment and open the live URL.
10. Test every page on the live project URL, not only locally.
11. Test desktop, mobile, keyboard navigation, Ask Dax, cross-page session persistence, quiz, YouTube, AI-video placeholder, CTA, images, links, and browser console.

Do not add canonical or `og:url` metadata until the repository owner and name are final. Then add the exact production URL to each page.

## Ask Dax
Ask Dax is a client-side educational knowledge-base chatbot, not a live generative model. It uses `sessionStorage` key `dutchShepherdAskDaxSessionV1`, requires no API key, and does not transmit conversations. Clear Conversation removes the session and restores the welcome state.

## Suitability Quiz
Eight required questions score 0–2 points each. Scores 13–16 produce “Potentially a Strong Match,” 8–12 produce “Consider Carefully,” and 0–7 produce “This Breed May Not Fit Your Current Lifestyle.” Results are educational, not professional placement advice.

## AI-Generated Video
Expected final files:
- `assets/video/dutch-shepherd-bite-work.mp4`
- `assets/video/dutch-shepherd-bite-work.webm`
- `assets/images/dutch-shepherd-video-poster.webp`
- `assets/captions/bite-work-captions.vtt`

The current media page deliberately shows a poster placeholder rather than a broken player. After adding and validating the MP4/WebM, replace the placeholder in `media.html` with the accessible HTML5 video element specified in the assignment. Update the supplied VTT cues so they accurately match the final video before representing captions as complete.

### Generation prompt
> Create a realistic, cinematic documentary-style video of a healthy adult brindle Dutch Shepherd performing a controlled working-dog bite-work exercise on a professional outdoor training field.
>
> The Dutch Shepherd has accurate breed characteristics, including an athletic build, upright ears, a brindle coat, balanced proportions, and realistic canine movement.
>
> A qualified adult handler gives clear commands and maintains control using appropriate professional equipment. A trained adult decoy wears complete padded protective bite equipment. The dog engages the protected equipment, maintains a controlled grip, releases when commanded, and returns under control to the handler.
>
> Show: 1. Handler and Dutch Shepherd waiting calmly 2. Decoy entering the controlled training area 3. Handler giving a working command 4. Dog engaging the protective equipment 5. Controlled grip 6. Handler giving the release command 7. Dog releasing 8. Dog returning calmly to the handler.
>
> Use a professional K9 or dog-sport training environment, natural daylight, realistic shadows, smooth camera movement, accurate canine anatomy, and documentary-style cinematography. The tone should be disciplined, athletic, educational, controlled, and ethical. Format: 16:9 landscape, 1080p, approximately 15–25 seconds. Do not include blood, injury, exposed-skin contact, unprotected people being bitten, uncontrolled aggression, children, crowds, police logos, weapons, text overlays, deformed anatomy, extra limbs, or unsafe handling.

## Future AI Integration
Conceptual architecture: GitHub Pages → Ask Dax interface → secure HTTPS endpoint → external serverless backend → AI provider → curated Dutch Shepherd knowledge. Suitable services include Azure Functions, Azure Static Web Apps API, Cloudflare Workers, Vercel Functions, or Netlify Functions. Credentials must stay in protected server-side environment variables, never public HTML, JavaScript, CSS, GitHub Pages, or a public repository. Add input validation, rate limiting, request timeouts, error handling, prompt-injection defenses, narrow content boundaries, curated retrieval, minimal collection, and privacy-conscious logging.

## Multimedia and Attribution
The homepage YouTube embed remains externally hosted and is credited to the original content owner. The hero/poster visual is AI-generated and disclosed on `sources.html`. Replace image placeholders only with licensed, accurately identified Dutch Shepherd images and add credits. The future video must retain its AI-content label, safety notice, poster, and accurate captions.

## Academic Sources
APA-style references and research boundaries appear on `sources.html`. Core facts are based primarily on FCI and AKC standards, with veterinary context from a veterinarian-reviewed PetMD guide.

## Accessibility
Semantic landmarks, one H1 per page, skip links, keyboard-ready navigation, visible focus, ARIA state for menus/chat, form labels, quiz error messaging, live regions, captions path, iframe title, responsive text, contrast, and `prefers-reduced-motion` are included.

## Deployment Testing
- Test all root HTML pages and `404.html`
- Test CSS/JS loading under the repository subdirectory
- Test hamburger open/close, Escape, and `aria-expanded`
- Test every internal and external link
- Test YouTube at multiple widths
- Test Ask Dax send, Enter, suggestions, fallback, clear, and cross-page persistence
- Test quiz validation, scoring, restart, and focus movement
- Test AI-media placeholder; after media is added, test MP4, WebM, poster, and captions
- Test `CLICK HERE NOW` opens the assigned URL in a new tab
- Test keyboard navigation, focus visibility, reduced motion, mobile safe areas, and browser console
- Run a case-sensitive path audit before publishing

## Academic Disclaimer
This website was created as an educational MBA project. It is not affiliated with or endorsed by any breed organization, veterinary organization, training organization, or other third party unless explicitly stated.
