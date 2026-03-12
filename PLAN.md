# PLAN.md - RBB Pertamina Prep

## Project Goal
Build a polished, bug-free quiz preparation web app for RBB Pertamina (Rekrutmen Bersama BUMN) targeting D3 Teknik Kimia - Operator position. The app should work flawlessly on mobile and desktop.

## Current State
- v1.0 is live on GitHub Pages
- 150 questions across 5 categories
- Core quiz, stats, and materials features working
- 32 issues found in code review (3 Critical, 7 High, 12 Medium, 10 Low)

## Task Breakdown

### Phase 1: Critical Bug Fixes (Priority: IMMEDIATE)
- [ ] C1: Fix timer leak in showPage() - add clearInterval(timerInterval) when navigating away
- [ ] C2: Add browser history management (pushState/popstate) so back button works
- [ ] C3: Add responsive breakpoints (@media queries for phone/tablet/desktop)

### Phase 2: High Priority Fixes
- [ ] H1: Hide bottom nav during quiz OR add navigation guards
- [ ] H2: Add updateHomeStats() call in confirmReset()
- [ ] H3: Fix modal-confirm empty onclick
- [ ] H4: Add basic accessibility (ARIA attributes, keyboard support, focus styles)
- [ ] H5: Use semantic HTML (header, nav, main, section)
- [ ] H6: Fix daily mode mixed scoring to use weighted average
- [ ] H7: Fix wrong count to include low-score TKP in daily mode

### Phase 3: Medium Priority Improvements
- [ ] M1: Pause timer during quit confirmation modal
- [ ] M2: Add click-outside-to-close on modal
- [ ] M3: Add Escape key to close modal
- [ ] M4: Shuffle answer options (with index remapping)
- [ ] M5: Deduplicate catNames into single global constant
- [ ] M6: Migrate inline onclick to addEventListener (long-term)
- [ ] M7: Fix secondary text color contrast for WCAG AA
- [ ] M8: Add try-catch to saveData()
- [ ] M9: Fix streak calculation (use ISO dates instead of locale-dependent)
- [ ] M10: Consider extracting questions to separate JSON (future)
- [ ] M11: Wrap initialization in DOMContentLoaded
- [ ] M12: Hide TKP score label for non-TKP quizzes

### Phase 4: Low Priority Polish
- [ ] L1: Remove dead isTKP code
- [ ] L2: Fix redundant ternary in autoTimeout
- [ ] L3: Dynamic question count badges
- [ ] L4: Fix progress bar to reach 100%
- [ ] L5: Replace alert() with styled modal for empty categories
- [ ] L6: Add back-to-results nav on review page
- [ ] L7: Add meta theme-color
- [ ] L8: Add favicon
- [ ] L9: Scope transition to specific properties
- [ ] L10: Add will-change hints for animations

### Phase 5: Future Enhancements
- [ ] Add more questions (target: 300+)
- [ ] Add timed full exam simulation mode
- [ ] Add progress sharing / screenshot results
- [ ] PWA support (offline mode, install prompt)
- [ ] Split questions into separate JSON files for lazy loading
