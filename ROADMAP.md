# Page Pals roadmap

Kids photograph a page from a real book, pick a buddy (caterpillar, bouncy ball, butterfly, or their own drawing), and read aloud. The buddy moves across the actual page only while they keep reading.

Live prototype: https://itagut.github.io/page-pals/

## Where the web prototype is today (version 13)

- Take a photo or upload one or more pages; uploaded pages queue up for "Next page"
- Word finding on the photo itself, so illustrations stay visible
- Grown-up check: fix spelling, skip a box, tap a missing word to have it read automatically, or drag a box around it
- Stray boxes in illustrations start skipped
- Pinch or +/- zoom on the photo while checking words
- Read-aloud tracking with kinder matching for children's speech, a "The app heard" line, and a microphone check
- Bouncy ball can bounce on voice beats (syllable-ish timing)
- Pause keeps the photo and position; "Zoom to the line" for small text
- End-of-page stats: words read, time, words per minute, help taps, tricky words
- Tap a word to hear it; Skip word for names the recognizer never gets

### Known limits of the web version

- Background noise disrupts listening (the browser's speech recognition can't be filtered or locked to one voice)
- White or light text on coloured pages can be missed (an extra pass was removed while fixing word finding; can come back)
- Syllable bounces are timed from loudness, not true syllable recognition
- Nothing is saved between sessions

## Next for the web prototype (validation)

- [ ] Real reading sessions with kids: do they ask to read again, does the buddy help or stress them
- [ ] Confirm listening works reliably on iPhone Safari in a quiet room
- [ ] Bring back the light-text pass, tested on real pages
- [ ] Parent interviews: would they pay, and how does it compare with Ello or Google Read Along

## Native app (React Native, iPhone, iPad and Android)

- [ ] **Voice isolation**: the child says a short sample to set up a voiceprint, and only her voice is followed; use the phone's built-in voice noise reduction
- [ ] **Book collections**: a parent scans every page ahead of time (for example before bedtime), fixes words once, and saves the book for the child to read and reread
- [ ] Pick up where they left off; reorder or rescan single pages
- [ ] Progress across rereads of the same book (words per minute and tricky words over time)
- [ ] True syllable-by-syllable tracking (on-device alignment of speech to the known text)
- [ ] Syllable-level accuracy report for parents (cloud pronunciation scoring as an option, with parental consent)
- [ ] Live camera mode with the buddy pinned to the physical book
- [ ] Keep photos and audio on the device (privacy, COPPA, copyright)

## Later ideas

- Practice words list from school, highlighted in any book
- Book content: publisher licensing, openly licensed children's books, or buying books in the app (Kindle and Libby don't let outside apps read their books)
- Apple TV dropped for now: no camera and awkward microphone input
