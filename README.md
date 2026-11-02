# The-Hobbyist-Club
CSC 111 Nile University Group Project

🔗 **[View Live Demo](https://ramy-elmasry.github.io/The-Hobbyist-Club/)**

---

# Action Plan & TODO List

**Target Files in Root:**
- [`index.html`](file:///home/cryptic256/code/web/The-Hobbyist-Club/index.html)

- [`about.html`](file:///home/cryptic256/code/web/The-Hobbyist-Club/about.html)

- [`style.css`](file:///home/cryptic256/code/web/The-Hobbyist-Club/style.css)

- [`cheatsheet.md`](file:///home/cryptic256/code/web/The-Hobbyist-Club/cheatsheet.md)

- [`README.md`](file:///home/cryptic256/code/web/The-Hobbyist-Club/README.md)


---

## 1. Project Navigation & Structural Integrity

- [x] **Fix Broken Football Link in `index.html`**

  - Updated `<a href="Omar A/">` to explicit `<a href="Omar A/index.html">Football</a>` to prevent 404s when opened locally (`file://`).
- [x] **Standardize Team and Page Counts in `index.html`**

  - Standardized to 6 team members and 14 total pages (2 root pages + 12 member subpages) across lines 25 and 61.
- [x] **Connect All Team Member Subpages in `about.html`**

  - Replaced dead `<a>` placeholders with live, descriptive links to both subpages for each member:
    - [x] **Jerome Benjamin:** `Jerome G/index.html` & `Jerome G/weekend.html`
    - [x] **Omar Ahmed Mohamed Wasfat:** `Omar A/index.html` & `Omar A/page2.html`
    - [x] **Omar Ahmed Salah Aldeen Nayel:** `Omar N/index.html` & `Omar N/page2.html`
    - [x] **Marogina Ashraf Samir:** `Marogina A/basics.html` & `Marogina A/types.html`
    - [x] **Ramy Abdallah Mohamed:** `Ramy A/index.html` & `Ramy A/page2.html`
- [x] **Remove Inappropriate Card in `about.html`**

  - Removed "Member 6 (dead / kia)" card to maintain academic professionalism.
- [x] **Add Two-Way Navigation to All Member Subpages (No "Trap" Pages)**

  - [x] **Jerome G:** Added `../index.html` (Main Home) to both pages.
  - [x] **Omar A:** Added `../index.html` (Main Home) alongside internal page navigation.
  - [x] **Omar N:** Added top `<nav>` with `../index.html` on both pages, cleaned up trailing `>` typo, and fixed internal player link.
  - [x] **Marogina A:** Added `../index.html` (Main Home) styled navigation buttons to both pages.
- [x] **Automated Link Verification**

  - Validated all anchor tags across all 11 HTML files; 100% of relative paths resolve cleanly without 404 errors.

---

## 2. Study & Oral Discussion Preparation

- [x] **Create Comprehensive Study Cheatsheet (`cheatsheet.md`)**

  - Documented every HTML tag used across the project with plain-English definitions.
  - Documented every CSS property, selector, and Box Model rule.
  - Documented directory path traversal rules (`../` vs `./`).
  - Added top 5 oral discussion questions with ready-to-recite answers for the viva.

---

## 3. Content & Text Cleanup

- [x] **Fix Section Heading in `index.html` (Line 30)**

  - Replaced `<h2>place holder text</h2>` with `<h2>Featured Hobbies</h2>`.
- [x] **Replace Placeholder Descriptions for Hobbies in `index.html`**

  - [x] **Formula 1 Card:** Added summary of F1 engineering, Ferrari, and race weekend dynamics.
  - [x] **Basketball Card:** Added summary of basketball teamwork, fast-paced play, and LeBron James.
  - [x] **Volleyball Card:** Added summary of indoor and beach volleyball dynamics and teamwork.
  - [x] **Football Card:** Added summary of football tactics, excitement, and teamwork.
- [x] **Refine Hero Section Text in `index.html`**

  - Removed placeholder text and clearly introduced the CSC 111 project portfolio.
- [x] **Replace Placeholders in `about.html`**

  - [x] Replaced placeholder under "About The Project" with university course details (CSC 111).
  - [x] Replaced placeholder under "Goal 1: Share Hobbies".
  - [x] Replaced placeholder under "Goal 2: Team Collaboration".

---

## 4. 6th Member Integration

- [x] **Receive 6th Member's Info**

  - Name: Yehia Shendy Yehia Shendy, Student ID: 261001243.
- [x] **Add 6th Member Card to `about.html`**

  - Added Yehia Shendy Yehia Shendy id: 261001243 with live links to his two subpages.
- [x] **Create 6th Member's 2 Hobby Pages (`Yehia S/`)**

  - `Yehia S/index.html`: Football basics, pitch diagram, and essential rules.
  - `Yehia S/page2.html`: Major tournaments (FIFA World Cup, Champions League) and football legends.
  - Embedded local images: `football_pitch.jpg` and `trophy.jpg`.
- [x] **Add 6th Member Hobby Card to `index.html`**

  - Added World Football card linking to `Yehia S/index.html`.

---

## 5. CSS Bonus Marks (1.5 Marks per Student)

- [x] **Ramy A:** Linked to shared `style.css` (qualifies).

- [x] **Omar A:** Internal CSS block in `<head>` (qualifies).

- [x] **Marogina A:** Internal CSS block in `<head>` (qualifies).

- [x] **Yehia S:** Internal CSS block in `<head>` (qualifies).

- [ ] **Jerome G:** Uncomment stylesheet link and fix relative path (`../style.css`) or add internal `<style>` rules.

- [ ] **Omar N:** Add CSS styling (either link to `../style.css` or add internal `<style>` block).

- [ ] **Jerome G:** Uncomment stylesheet link and fix relative path (`../style.css`) or add internal `<style>` rules.

- [ ] **Omar N:** Add CSS styling (either link to `../style.css` or add internal `<style>` block).


---

## 6. Global Styling Enhancements (`style.css`)

- [ ] **Add Link Styling for Subpage Navigators**

  - Ensure links inside `.card a` have clear visual distinction (underlines, color accents, hover states).
- [x] **Add Responsive Image Rules**

  - Added `img { max-width: 100%; height: auto; display: block; margin: 15px auto; border-radius: 6px; }` to support responsive images across subpages.
- [ ] **Add Table Styling**

  - Add `table { width: 100%; border-collapse: collapse; margin-top: 10px; }` to improve formatting for tables used in subpages.

---

## 7. Final Submission Checklist (Deadline: 31 October 2026)

- [ ] All team members verify their subpages render properly in standard browsers.

- [ ] Remove all remaining placeholder texts and debug comments.

- [ ] Package entire project into ONE `.zip` file containing all root files, stylesheets, and member folders with assets.

- [ ] Every team member submits the `.zip` file individually on the portal before October 31.
