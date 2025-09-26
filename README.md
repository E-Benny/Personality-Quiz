# Quiz App — Two-Column Card Interface

An interactive quiz web app built with **HTML, CSS, and Vanilla JavaScript**.  
It uses a pastel two-column card layout with images, radio options, and navigation buttons.  

**Live demo:** [View on CodePen](https://codepen.io/E-Benny/pen/YPwXZXz)

---

## Features

- **Two-Column Layout**  
  - Left panel: step counter and question text.  
  - Right panel: image, answer options, and navigation buttons.  

- **Dynamic Questions**  
  - Questions, answer options, and images are stored in a JavaScript array.  
  - Each step is rendered dynamically into the DOM.  

- **Radio Option Selection**  
  - Users select one answer per question.  
  - Selected values are stored in an `answers` array.  

- **Navigation Buttons**  
  - Previous → go back to the last question.  
  - Next / Finish → move forward or complete the quiz.  

- **Completion Summary**  
  - After finishing, the app shows a thank-you card with a summary of all answers.  

---

## UI & Styling

- **Background**: Animated GIF with a pastel fallback color.  
- **Typography**:  
  - Titles → Orbitron.  
  - Inputs & labels → Exo 2.  
- **Colors**:  
  - Left panel: light blue (`#e6f2ff`).  
  - Right panel: white with subtle blue accents.  
- **Buttons**: Rounded, with hover and disabled states.  
- **Responsive**: Max width `900px`, centered with flexbox.  

---

## Code Structure

### HTML
- `.quiz-container` → wraps the quiz card.  
- `.quiz-card` → grid with left and right columns.  
- `.quiz-left` → displays the step counter and question.  
- `.quiz-right` → displays image, answer options, and navigation buttons.  

### CSS
- Global background, font families, and pastel theme.  
- `.quiz-card` → rounded card with a grid layout.  
- `.question-image` → object-fit with custom object-position for vertical alignment.  
- `.option-item` → styled radio labels with hover and active states.  
- `.nav-button` → interactive navigation buttons with hover/disabled states.  
- `.thank-you-card` → shown after the quiz, contains answer summary.  

### JavaScript
- `quiz` → array of objects holding question text, options, and image URLs.  
- `answers` → stores user’s selected answers.  
- `renderQuestion()` → dynamically renders the current question, options, and image.  
- `showSummary()` → displays thank-you card with answer summary.  
- Event listeners for Previous and Next/Finish navigation.  
- `renderQuestion()` is called initially to load the first step.  

---

## How to Run

1. Clone or download this repo.  
2. Open the `.html` file in any browser.  
3. Or, try it live here → [CodePen Demo](https://codepen.io/E-Benny/pen/YPwXZXz).  

---

## Developer Notes

- Code is fully commented for clarity (HTML, CSS, JS).  
- All options and images are easily customizable in the `quiz` array.  
- No external libraries required — pure **vanilla JS + CSS**.  
