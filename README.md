how to do blog?

toggling btwn languages in profile section makes it bounce; fix it

1. Scroll-triggered section reveals — right now sections just appear as you scroll. Adding a subtle fade-up animation as each section enters the viewport (the way the hero does) would make the whole site feel more alive and intentional. About 10 lines of JS with IntersectionObserver.
2. Active nav highlight — as you scroll past each section, the corresponding nav link lights up in red. Very useful on a long single-page site and makes it feel polished.
3. Gallery image captions that slide up on hover — the caption text is currently always visible. It would look cleaner if captions were hidden and slid up when you hover over the main image.

4. Smooth scroll-to-section with offset — clicking a nav link currently jumps to the section but the fixed nav bar partially covers the heading. A small JS offset fix would make it land perfectly.
5. "Back to top" button — a small gold arrow that appears after scrolling down, fixed in the bottom-right corner. Common on Japanese sites and useful for single-page layouts.
6. Hover effect on achievement cards — a subtle gold left-border slide-in or background shift when hovering each card, making the dark section feel more interactive.
7. Stat counter animation — instead of "1×", "5×", "7×", "3×" just sitting there, they could count up from 0 when the red bar scrolls into view. Very satisfying.

8. Image lightbox for gallery — clicking the main gallery image opens it full-screen with a dark overlay. Good for desktop users who want a closer look at the competition photos.
9. Subtle parallax on hero image — the photo scrolls slightly slower than the page as you scroll down, creating a depth effect. One line of JS.
10. Page loading screen — a brief 1-second splash with just the dojo name/mark in Japanese before the hero loads in. Very common on Japanese design sites and sets the tone immediately.
11. Transition between EN/JP toggle — instead of text swapping instantly, a very quick crossfade (150ms opacity) when switching languages would feel smoother.
