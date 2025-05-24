# Text-to-Speech-Converter

The goal of this project is to create a client-side web application that allows users to enter text and convert it into spoken words using the Web Speech API. This type of application can be useful for visually impaired users, language learners, or accessibility tools.

🧩 Components
1. HTML (Structure)
-> The HTML defines the layout and elements of the page.

-> Major components:

                  * <textarea>: Where users enter text.

                  * <button>: Triggers the text-to-speech conversion.

                  * <p>: Displays error messages if the text area is empty.

2. CSS (Styling)
-> CSS styles the UI to make it responsive and visually appealing.

-> A gradient background, rounded buttons, and consistent fonts (via Google Fonts) improve user experience.

3. JavaScript (Functionality)
-> JavaScript handles the logic for the conversion:

* Captures user input.

* Checks if the text is not empty.

* Uses SpeechSynthesisUtterance to generate speech from text.

* Updates the UI dynamically (e.g., changes button text, displays errors).

🗣️ Web Speech API
-> Key Concepts:
            * window.speechSynthesis: The interface to control the speech synthesis engine.

            *SpeechSynthesisUtterance(text): Creates an utterance object from the provided text.

            *speechSynthesis.speak(utterance): Speaks the utterance.

            *This API works directly in most modern browsers without needing extra libraries or servers.

🔄 Workflow
-> User Inputs Text: Enters text in the text area.

-> Clicks Button: Triggers JavaScript event listener.

-> Validation: Checks if input is empty.

-> Speech Playback:

                  * If valid: Text is converted and spoken aloud.

                  * If invalid: Error message is shown.
 
-> Feedback: Button text temporarily changes to indicate speech is playing.

⚙️ Advantages
-> Simple and Lightweight: No server or database is needed.

-> Native Browser API: Ensures speed and privacy (no external API calls).

-> Accessibility Friendly: Useful for users who prefer or require audio feedback.

🔐 Limitations
-> Relies on browser support; older browsers may not function correctly.

-> No control over voice selection, speed, or pitch in this version.

-> Cannot export audio output as a file.

🧭 Applications
-> Reading tools for the visually impaired

-> Pronunciation assistance for language learners

-> Educational apps

-> Screen readers and accessibility enhancers
