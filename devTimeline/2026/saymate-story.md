# 📝 The Story Behind SayMate: How We Built an App to Give Everyone a Voice

Building an app is always an adventure, but building one with the person you love is something truly special. 

Recently, my fiancée (who is a UI/UX Analyst) and I launched **SayMate** on the Google Play Store. She crafted the beautiful, accessible interface, while I handled all the development. Together, we wanted to build a simple, free AAC (Augmentative and Alternative Communication) app to help non-verbal individuals, kids, and speech therapy students communicate using visual flashcards.

Here is the story of how SayMate went from a simple conversation at our kitchen table to a live product in production.

---

## 🧠 1. The Brainstorming & Design: Why SayMate?

The idea for SayMate came from a simple observation: **communication should be a basic human right, accessible to everyone.**

While researching speech and language development tools, we wanted to create something that was as friendly, simple, and direct as possible. We set out to design an app that is:
1. **Completely free and accessible** with no subscription fees or paywalls.
2. **Clean and quiet**, without ads or complicated settings that might distract a child.
3. **Highly customizable**, allowing families to use familiar faces and voices.

As a UI/UX Analyst, my fiancée immediately focused on **simplicity and accessibility**. She drafted a layout around our core philosophy: **Image ➔ Label ➔ Voice ➔ Tap ➔ Speak.**

We also realized that speech learning works best when it's interactive. So, we brainstormed a way to reinforce vocabulary through play—leading to our built-in **"Guess the Image"** word-scramble mini-game, complete with celebratory confetti and sound effects.

---

## 🛠️ 2. The Tech Stack: Local-First and Responsive

Because we wanted SayMate to be fast, reliable, and run smoothly on older devices, we made a crucial architectural choice: **Local-First.** The app does not rely on databases in the cloud, logins, or active internet connections. 

Here is what we chose to power the app:

* **Framework:** **Flutter (Dart)** – We chose Flutter because it allowed us to build a gorgeous, fluid, and responsive visual grid system that performs beautifully.
* **Audio Recording & Playback:** We used `record` for capturing custom high-quality voice audio and `audioplayers` for crisp instant playback when a card is tapped.
* **Text-to-Speech:** Integrated `flutter_tts` as a seamless fallback, letting the app speak labels automatically if no custom voice is recorded.
* **Storage:** We used `shared_preferences` and the local file system (via `path_provider`) to save card metadata, categories, and media. Everything stays 100% private on the user’s phone.
* **User Engagement:** We used `confetti` and native sound effects to create a rewarding experience in the vocabulary game.

---

## 🧪 3. The Testing: Real Feedback from Real People

Building the app was only half the battle. Testing it was where the real magic happened.

We set up a **Closed Testing** release on the Google Play Store and invited a group of amazing testers, including parents, educators, and close friends. Their real-world feedback was eye-opening:
* **Simplicity is Key:** Early layouts had buttons that were too small for children or motor-impaired individuals. Using my fiancée's UI/UX expertise, we immediately redesigned the home screen to feature a clean, large grid with generous tap targets.
* **Familiar Voices Matter:** We realized that children responded far better to hearing their parents’ or teachers' voices than a standard robotic voice. This pushed us to perfect our local audio recording feature.
* **Import/Export Tool:** Therapists wanted a way to move customized flashcard sets between devices. Thanks to this feedback, we added a secure zip-based backup and restore tool.

We are incredibly grateful to all our testers who broke the app, suggested features, and helped us make it rock-solid!

---

## 🚀 What's Next?

SayMate is currently live and 100% free on the [Google Play Store](https://play.google.com/store/apps/details?id=com.mreycode.say_mate) for Android. 

While it is Android-only for now, our long-term goal is to bring it to iOS and Huawei users so more families can benefit. 

Building SayMate together has been an incredibly rewarding project for both of us. We hope it brings comfort, learning, and a clear voice to the people who need it most. ❤️
