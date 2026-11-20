# Experiment-3.1 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-3.1
# Experiment-3.1

## Understanding Natural Language Processing and Speech AI with Microsoft Tools.

##  CO5

##

## Aim

To study the concept of speech-enabled AI applications and understand how speech recognition and speech synthesis are used to create intelligent voice-based systems.

## Objectives

The objectives of this experiment are:

- To understand the meaning of speech-enabled AI solutions.

- To study the working of speech recognition or speech-to-text technology.

- To study the working of speech synthesis or text-to-speech technology.

- To understand the role of speech technologies in conversational AI systems.

- To identify the real-world applications, advantages, and limitations of speech-enabled AI systems.

## Theory

Speech is one of the most natural and important methods of human communication. Humans normally communicate with each other through spoken language, and when the same ability is added to AI applications, machines become easier and more natural to use. Speech-enabled AI solutions allow users to interact with computers, mobile applications, smart devices, and AI agents using voice commands instead of typing text or clicking buttons.

Speech-enabled solutions mainly depend on two important technologies: speech recognition and speech synthesis. Speech recognition converts spoken words into written text, while speech synthesis converts written text into spoken audio. These two technologies work together to create voice-based AI systems such as virtual assistants, customer service bots, smart speakers, navigation systems, healthcare dictation tools, and e-learning platforms.

Speech capabilities make AI applications more accessible and user-friendly. They are especially useful for people with visual impairments, reading difficulties, or mobility challenges. They also help users perform tasks hands-free, such as giving voice commands while driving, cooking, working, or using smart devices. Speech technologies can support multiple languages and dialects, which helps AI systems reach a wider audience.

## Speech-Enabled AI Solutions

Speech-enabled AI solutions are applications that can understand spoken input or generate spoken output, as shown in Figure 1. These systems make human-computer interaction more natural because users can communicate with machines in the same way they communicate with people.

For example, when a user says, “What is the weather today?”, a voice assistant listens to the spoken command, converts it into text, processes the meaning, retrieves the answer, and then speaks the response back to the user. This complete process involves speech recognition, natural language processing, and speech synthesis.

Speech-enabled AI solutions are useful in many areas. In customer service, they can transcribe customer calls, route callers to the correct department, and support automated voice responses. In education, they can read lessons aloud and help students with different learning needs. In healthcare, doctors can dictate patient notes instead of typing them manually. In accessibility tools, speech systems can read documents and websites aloud for visually impaired users.

The main goal of speech-enabled AI is to make technology easier, faster, and more inclusive for users.

Figure 1: Speech-enabled voice assistant system.

## Speech Recognition

Speech recognition is also called speech-to-text. It is the process of converting spoken language into written text as shown in Figure 2. This technology allows AI systems to listen to human speech and convert it into a form that computers can process.

For example, when a person says, “Open the calendar,” the speech recognition system converts the spoken sentence into written text: “Open the calendar.” After that, the AI system can understand the command and perform the required action.

Speech recognition is used in voice assistants, call centers, meeting transcription tools, healthcare documentation systems, smart home devices, and language learning applications.

Figure 2: Speech recognition processing pipeline.

## Working of Speech Recognition

Speech recognition works through a series of stages. Each stage plays an important role in converting sound into accurate text.

## 1. Audio Capture

The first stage is audio capture. In this stage, a microphone records the user’s voice. Human speech is produced as sound waves, but computers cannot directly understand sound waves. Therefore, the microphone converts the analog sound waves into digital signals.

The quality of audio capture is very important. If there is background noise, poor microphone quality, or the speaker is too far from the microphone, the accuracy of speech recognition may decrease. Clear audio input improves the performance of the system.

## 2. Pre-Processing

After audio capture, the recorded audio is cleaned and prepared for further processing. This stage is called pre-processing. The system may remove background noise, unwanted clicks, hums, and other disturbances from the audio signal.

Pre-processing helps the system focus only on useful speech information. It improves the quality of input given to the speech recognition model.

## 3. Feature Extraction

Raw audio contains a large amount of information. It is difficult for the AI model to process raw audio directly. Therefore, the system extracts important features from the audio signal.

One common method used for feature extraction is Mel-Frequency Cepstral Coefficients, also called MFCC. MFCC represents the important characteristics of speech in a compact numerical form. It is inspired by the way the human ear hears sound. MFCC focuses more on the frequency ranges that are important for human speech.

In simple words, MFCC helps convert the speech signal into useful numbers that the machine learning model can understand.

## 4. Acoustic Modeling

Acoustic modeling is the stage where the system identifies the sounds present in speech. These small sound units are called phonemes. A phoneme is the smallest unit of sound that can change the meaning of a word.

For example, the word “cat” contains three phonemes: /k/, /æ/, and /t/. The acoustic model studies the extracted audio features and predicts which phonemes are being spoken.

Modern speech recognition systems use deep learning models such as transformer-based models. These models can understand speech patterns more accurately by analyzing the surrounding audio context. This helps the system recognize words even when pronunciation, accent, or speaking speed varies.

## 5. Language Modeling

After identifying phonemes, the system uses language modeling to predict the most meaningful word sequence. Language models understand vocabulary, grammar, sentence structure, and common word patterns.

This stage is important because some words sound the same but have different meanings. For example, “their” and “there” have similar pronunciations, but their meanings are different. The language model uses context to select the correct word.

For example, in the sentence “The weather is nice,” the model can understand that “weather” is more suitable than “whether.”

## 6. Decoding

Decoding is the process of selecting the best possible text output from many possible word combinations. The system compares different possibilities and chooses the sentence that best matches the audio input and language rules.

For example, if the user says, “Please send the report by Friday,” the decoder may compare different possible sentences and finally select the most accurate one.

## 7. Post-Processing

The final stage is post-processing. In this stage, the raw text is improved and formatted properly. The system adds capitalization, punctuation, number formatting, and other corrections.

For example, raw output like “hello my name is sam” can be converted into “Hello, my name is Sam.” Similarly, “three p m” can be converted into “3 PM.”

Post-processing makes the output easier to read and understand.

## Speech Synthesis

Speech synthesis is also called text-to-speech. It is the process of converting written text into spoken audio. This technology allows AI systems to speak responses to users, as shown in Figure 3.

For example, if the text is “Your appointment is at 3 PM,” the speech synthesis system converts this text into natural-sounding speech.

Speech synthesis is used in virtual assistants, chatbots, navigation systems, screen readers, e-learning platforms, audio notifications, and entertainment applications.

## Figure 3: Text-to-speech synthesis process.

## Working of Speech Synthesis

Speech synthesis also works through several stages. These stages convert written text into meaningful and natural-sounding voice output.

## 1. Text Normalization

The first stage of speech synthesis is text normalization. In this stage, the system converts written symbols, abbreviations, dates, numbers, and special characters into spoken form.

For example, the sentence “Dr. Smith ordered 3 items for $25.50” is converted into “Doctor Smith ordered three items for twenty-five dollars and fifty cents.”

Text normalization is important because computers must know how to pronounce numbers, abbreviations, and symbols properly. Without normalization, the speech may sound unnatural or incorrect.

## 2. Linguistic Analysis

After normalization, the system performs linguistic analysis. In this stage, the text is divided into words, syllables, and phonemes. The system analyzes how each word should be pronounced.

This stage may use pronunciation dictionaries and AI models to decide the correct pronunciation of words. It is especially important in English because spelling and pronunciation are often different.

For example, the words “though,” “through,” and “cough” contain similar letters, but they are pronounced differently.

## 3. Grapheme-to-Phoneme Conversion

Grapheme-to-phoneme conversion, also called G2P conversion, converts written letters into sound units. A grapheme is a written letter or group of letters, and a phoneme is a sound unit.

For example, the word “phone” is written with the letters “p-h-o-n-e,” but it is pronounced using the /f/ sound at the beginning. The G2P system helps the AI model decide the correct sound for each word.

Modern speech synthesis systems use neural networks to perform G2P conversion more accurately, especially for proper names, uncommon words, and regional pronunciations.

## 4. Prosody Generation

Prosody means the natural rhythm, pitch, stress, pauses, and intonation used in speech. Prosody is very important because it makes speech sound human-like.

A sentence can have different meanings depending on how it is spoken. For example, the sentence “I never said he ate the cake” can express different meanings depending on which word is stressed.

Prosody generation decides where to pause, which words to emphasize, how fast to speak, and whether the pitch should rise or fall. Without proper prosody, the voice may sound robotic or flat.

## 5. Audio Waveform Generation

The final stage is audio waveform generation. In this stage, the system produces the actual speech audio. Modern systems use neural vocoders such as WaveNet, WaveGlow, and HiFi-GAN to generate high-quality and natural-sounding speech.

The system converts phoneme and prosody information into audio signals. These signals are then played through speakers or headphones so that the user can hear the spoken output.

## Combining Speech Recognition and Speech Synthesis

Speech recognition and speech synthesis are often combined to create conversational AI systems. Speech recognition allows the system to listen and understand the user’s spoken input. Speech synthesis allows the system to respond using spoken output.

For example, in a voice assistant:

The user says, “Set an alarm for 6 AM.”

The system uses speech recognition to convert this voice command into text.

The AI system understands the command and sets the alarm.

Then speech synthesis is used to reply, “Your alarm has been set for 6 AM.”

This combination creates a two-way conversation between humans and machines. It is used in smart speakers, IVR systems, customer service bots, language learning apps, and voice-controlled vehicles.

## Figure 4: Voice interaction flow using speech recognition, natural language processing, and text-to-speech.

##

## Real-World Applications

Speech recognition and speech synthesis are used in many real-world applications.

## 1. Voice Assistants

Voice assistants such as Siri, Alexa, and Google Assistant use speech recognition to understand user commands and speech synthesis to reply. Users can ask questions, set reminders, play music, check the weather, and control smart devices using voice.

## 2. Customer Service

Call centers use speech recognition to transcribe customer calls and analyze customer issues. Speech synthesis is used in automated phone systems to guide customers through options.

## 3. Meeting Transcription

Speech recognition is used to convert meetings, interviews, and lectures into written notes. This saves time and helps create searchable records.

## 4. Healthcare Documentation

Doctors and healthcare professionals use speech recognition to dictate patient notes. This reduces typing work and allows doctors to focus more on patient care.

## 5. Accessibility Tools

Speech synthesis helps visually impaired users by reading text aloud. It also supports users with reading difficulties such as dyslexia.

## 6. E-Learning

Educational platforms use speech synthesis to create narrated lessons, audio learning materials, and pronunciation examples. Speech recognition can also be used to evaluate spoken answers and language practice.

## 7. Navigation Systems

Navigation apps use speech synthesis to speak directions, alerts, and route updates. This allows users to receive information without looking at the screen.

## 8. Smart Home Devices

Smart home systems use speech recognition to accept commands such as turning lights on, adjusting temperature, or playing music.

## Code

# Install only the required libraries

!pip -q install SpeechRecognition gTTS

!apt-get -qq install ffmpeg > /dev/null

import subprocess

import speech_recognition as sr

from gtts import gTTS

from google.colab import files

from IPython.display import Audio, display

def assistant():

print("Upload a short voice recording: WAV, MP3 or M4A")

uploaded = files.upload()

if not uploaded:

print("No recording uploaded.")

return

filename = next(iter(uploaded))

# Convert the recording to a compatible WAV file

result = subprocess.run(

["ffmpeg", "-y", "-i", filename,

"-ar", "16000", "-ac", "1", "-c:a", "pcm_s16le",

"/tmp/voice_input.wav"],

capture_output=True

)

if result.returncode != 0:

print("Could not open this audio file. Try WAV or MP3.")

return

# Voice to text

recognizer = sr.Recognizer()

recognizer.operation_timeout = 20

try:

with sr.AudioFile("/tmp/voice_input.wav") as source:

recording = recognizer.record(source)

text = recognizer.recognize_google(

recording, language="en-IN"

)

print("You said:", text)

except sr.UnknownValueError:

print("Speech was unclear. Try a clearer recording.")

return

except sr.RequestError as error:

print("Speech service error:", error)

return

# Choose an answer

question = text.lower()

if "hello" in question:

reply = "Hello! Welcome to our AI class."

elif "your name" in question:

reply = "I am your classroom voice assistant."

elif "artificial intelligence" in question:

reply = "AI helps computers perform tasks that require intelligence."

else:

reply = "You said: " + text

print("Assistant:", reply)

# Text to voice

try:

gTTS(reply, lang="en").save("/tmp/reply.mp3")

display(Audio("/tmp/reply.mp3", autoplay=True))

except Exception as error:

print("Could not generate speech:", error)

assistant()

## Practice Task Questions

Write a short note on speech-enabled AI solutions.

Differentiate between speech recognition and speech synthesis.

Explain the working of speech recognition in simple words.

Write the main stages involved in the speech recognition process.

Explain the role of MFCC in speech recognition.

What are phonemes? Explain with one example.

Explain the working of speech synthesis in simple words.

What is text normalization? Give one example.

Explain the importance of prosody in speech synthesis.

Write five real-world applications of speech-enabled AI systems.

## Video Links

Creating Speech-Enabled Apps with Azure AI Services

Recognize & Synthesize Speech with Azure AI Speech Service

How Does Speech Recognition Work? Learn about Speech to Text, Voice Recognition and Speech Synthesis

Azure AI Speech Explained — Speech Recognition

Microsoft Azure AI Services—Get Started With Text-To-Speech

## Additional Resources

Azure Speech Documentation

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/

What is Azure Speech?

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/overview

Speech-to-Text Documentation — Azure AI Speech

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/index-speech-to-text

Text-to-Speech Documentation — Azure AI Speech

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/index-text-to-speech

Text-to-Speech Overview — Azure AI Speech

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech

About the Speech SDK — Azure AI Speech

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-sdk

Azure Speech SDK Samples — GitHub

URL: https://github.com/Azure-Samples/cognitive-services-speech-sdk

Azure AI Speech Product Page

URL: https://azure.microsoft.com/en-us/products/ai-foundry/tools/speech

Google Cloud Speech-to-Text

URL: https://cloud.google.com/speech-to-text

Text-to-Speech Technology: What It Is and How It Works

URL: https://www.readingrockets.org/topics/assistive-technology/articles/text-speech-technology-what-it-and-how-it-works

## Text Books

Speech and Language Processing

Authors: Daniel Jurafsky and James H. Martin

PDF/Access Link: https://web.stanford.edu/~jurafsky/slp3/ed3book.pdf

Useful for: Speech recognition, language modelling, NLP, and modern AI-based language systems.

Speech and Language Processing — Official Book Page

Authors: Daniel Jurafsky and James H. Martin

PDF/Access Link: https://web.stanford.edu/~jurafsky/slp3/

Useful for: Updated chapters on speech recognition, language models, and NLP concepts.

Speech Signal Processing by Praat

Author: David Weenink

PDF/Access Link: https://www.fon.hum.uva.nl/david/sspbook/sspbook.pdf

Useful for: Basic speech signal processing, waveform analysis, pitch, formants, and speech features.

Introduction to Digital Speech Processing

Author: Lawrence R. Rabiner

PDF/Access Link: https://elupu.utcluj.ro/wp-content/uploads/2024/03/Rabiner.pdf

Useful for: Digital speech processing, speech production, speech analysis, and speech recognition basics.

Fundamentals of Speech Recognition

Authors: Lawrence Rabiner and Biing-Hwang Juang

PDF/Access Link: https://external.dandelon.com/download/attachments/dandelon/ids/DE0066927926FFD6878FAC1257A3600449F90.pdf

Useful for: Speech recognition pipeline, acoustic modeling, language modeling, and recognition systems.

## Reference Books / Reference Resources

Spoken Language Processing: A Guide to Theory, Algorithm, and System Development

Authors: Xuedong Huang, Alex Acero, and Hsiao-Wuen Hon

Access Link: https://www.microsoft.com/en-us/research/publication/spoken-language-processing/

Useful for: Speech recognition, speech synthesis, spoken dialogue systems, and real-world speech applications.

Springer Handbook of Speech Processing

Editors: Jacob Benesty, M. M. Sondhi, and Yiteng Huang

PDF/Access Link: https://jontalle.web.engr.illinois.edu/Public/HandbookSpeechProcessing.08.pdf

Useful for: Advanced speech processing, speech coding, recognition, synthesis, and speaker analysis.

Neural Text-to-Speech Synthesis

Authors: Xu Tan and others

Access Link: https://link.springer.com/book/10.1007/978-981-99-0827-1

Useful for: Modern neural TTS, deep learning-based speech synthesis, and vocoder-based speech generation.

Text-to-Speech Synthesis — Cambridge Core Chapter

Author: Paul Taylor

Access Link: https://www.cambridge.org/core/books/texttospeech-synthesis/introduction/0F0A5AE0427A0B4EBB779B634CF77752

Useful for: Basic understanding of text-to-speech systems, pronunciation, prosody, and synthesis process.

Azure AI Speech Documentation

Publisher: Microsoft Learn

Access Link: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/

Useful for: Practical implementation of speech-to-text, text-to-speech, speech SDK, and AI speech services.

---


## 🖥️ PRESENTATION SLIDES


# Experiment-3.1 - All Lecture Slides Text


## Exp 3.1
### Slide 1
- UNIVERSITY INSTITUTE OF
- ENGINEERING
- DEPARTMENT OF ENGINEERING FOUNDATION-2
- PROGRAM
- NAME
- :
- Bachelor
- of Engineering
- SPECIALIZATION
- :
- COMPUTER SCIENCE & ENGINEERING
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 3                   Experiment No.3.1
- Topic
- : Understanding Natural Language Processing and Speech AI Concepts with Microsoft
- Tools
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- After
- completing this experiment, students will be able to
- :
- Understand the concept of speech-enabled AI applications
- .
- Study the working of speech recognition or speech-to-text technology
- .
- Understand the working of speech synthesis or text-to-speech technology
- .
- Identify the role of speech technologies in conversational AI systems
- .

### Slide 3
- Recap
- of Previous Experiment
- Text analysis is an important application of Artificial Intelligence and Natural Language Processing.
- Tokenization breaks text into smaller units called tokens.
- Frequency analysis, Bag-of-Words, and TF-IDF are statistical techniques for text representation.
- Text Rank is used for extractive summarization and keyword extraction.
- Semantic language models use embedding's to understand meaning and context.
- Text analysis is useful in sentiment analysis, spam detection, Chabot's, search engines, and summarization.

### Slide 4
- Figure-1 :
- Speech Processing Workflow using NLP
- Source
- :
- https://www.linkedin.com/pulse/speech-recognition-synthesis-next-frontier-conversational-cjiyc/
- Speech Recognition and Speech Synthesis
- in
- AI
- Topic(s
- )
- Introduction to Speech AI
- Speech-to-Text and Automatic Speech Recognition
- Text-to-Speech and Speech
- Synthesis
- Combining Speech Recognition
- and
- Speech Synthesis

### Slide 5
- Figure-2:
- Next-Generation Voice Assisted
- Solutions
- Source:
- https
- ://embeddedcomputing.com/technology/
- ai
- -machine-learning/computer-vision-speech-processing/next-generation-voice-assisted-solutions
- Speech-enabled AI solutions allow users to interact with machines using voice commands
- .
- These systems make human-computer interaction more natural because humans commonly communicate through spoken language
- .
- Speech-enabled AI applications use voice input and voice output to support intelligent interaction
- .
- Examples include voice assistants, smart speakers, customer service bots, navigation systems, healthcare dictation tools, and e-learning platforms.
- Speech-Enabled AI Solutions

### Slide 6
- Speech is one of the most natural forms of human communication
- .
- Speech AI helps users perform tasks hands-free while driving, cooking, working, or using smart devices
- .
- It also improves accessibility for visually impaired users, people with reading difficulties, and users with mobility challenges.
- Figure-3
- :Benefits of AI Communication for Speech Therapy
- Source:
- https
- ://emitrr.com/blog/
- ai
- -for-speech-therapy/
- Importance of Speech in AI

### Slide 7
- Speech recognition is also called
- speech-to-text
- .
- It is the process of converting spoken language into written text
- .
- For example, when a user says, “Open the calendar,” the system converts the speech into text: “Open the calendar
- .”
- Figure-4
- :Speech Recognition
- Source:
- https
- ://nordvpn.com/blog/what-is-speech-recognition/?
- srsltid
- =AfmBOopjpbgTA9UZ6fC33XUfJfo5WIDIZ-5JxMTGrCnKwZB-kuxsgJS8
- Speech Recognition

### Slide 8
- Speech recognition works through different stages
- :
- First, the microphone captures the user’s voice as an audio signal.
- Then pre-processing removes background noise and improves the quality of the audio.
- Feature extraction converts the audio signal into useful numerical features such as MFCC.
- The acoustic model identifies small sound units called phonemes.
- The language model predicts the most meaningful sequence of words.
- Finally, decoding and post-processing generate properly formatted text with punctuation and capitalization.
- Figure-5
- :Working of Speech Recognition
- Source:
- https
- ://www.techtarget.com/searchcustomerexperience/definition/speech-recognition
- Working of Speech Recognition

### Slide 9
- Speech synthesis is also called
- text-to-speech
- .
- It is the process of converting written text into spoken audio
- .
- For example, the text “Your appointment is at 3 PM” can be converted into natural-sounding speech
- .
- Figure-6
- :Speech
- Synthesis
- Source:
- https
- ://en.wikipedia.org/wiki/
- Speech_synthesis
- Speech Synthesis

### Slide 10
- Speech synthesis converts text into speech through several stages.
- Text normalization converts symbols, numbers, dates, and abbreviations into spoken form.
- Linguistic analysis divides the text into words, syllables, and phonemes.
- Grapheme-to-phoneme conversion changes written letters into sound units.
- Prosody generation adds rhythm, pitch, stress, pauses, and intonation.
- Finally, audio waveform generation creates the final speech audio using modern neural
- vocoders
- .
- Figure-7 :
- Working of Speech Synthesis
- Source:
- https
- ://www.researchgate.net/publication/304601298_Development_of_Text-to-Speech_Synthesizer_for_Pali_Language/figures?lo=1
- Working of Speech Synthesis

### Slide 11
- Speech recognition and speech synthesis are often combined to create conversational AI systems.
- Speech recognition helps the system listen to the user’s spoken input.
- Natural Language Processing helps the system understand the meaning of the input.
- Speech synthesis helps the system respond using spoken output.
- Example:
- The user says, “Set an alarm for 6 AM.”
- The system converts speech into text, understands the command, sets the alarm, and replies, “Your alarm has been set for 6 AM.”
- Figure-8 :
- Combining Speech Recognition
- and Speech Synthesis
- Source:
- https
- ://iprobe.cse.msu.edu/
- project_detail.php?id
- =20&?title=DeepTalk:_Vocal_Style_Encoding_for_Speaker_Recognition_and_Speech_Synthesis
- Combining Speech Recognition
- and
- Speech Synthesis

### Slide 12
- Summary of the
- Experiment
- Speech-enabled AI applications allow users to interact with machines using voice.
- Speech recognition converts spoken language into written text.
- Speech synthesis converts written text into spoken audio.
- Together, speech recognition, NLP, and speech synthesis create conversational AI systems.
- These systems are widely used in voice assistants, customer support, healthcare, education, accessibility tools, navigation, and smart homes
- .

### Slide 13
- Next
- Experiment
- T
- opic(s)
- Topic 1: Computer
- Vision
- Topic
- 2: Image
- Classification
- Topic
- 3: Object
- Detection
- Topic
- 4: Optical Character
- Recognition

### Slide 14
- Quiz/ FAQ’s
- What is speech-enabled AI?
- What is speech recognition?
- What is speech synthesis?
- What is the difference between speech-to-text and text-to-speech?
- Why is pre-processing important in speech recognition?
- What is the role of NLP in conversational AI?
- Give two real-world applications of speech-enabled AI.
- Why is speech AI important for accessibility?

### Slide 15
- R
- eferences/ Articles/ Videos
- References / Articles
- Microsoft Learn — Introduction to Azure AI Speech
- https://learn.microsoft.com/en-us/azure/ai-services/speech-service/overview
- Microsoft Learn — Speech to Text
- https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-to-text
- Microsoft Learn — Text to Speech
- https://
- learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech
- Videos
- How Does Speech Recognition Work? Speech-to-Text, Voice Recognition and Speech Synthesis
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://www.youtube.com/watch?v=6altVgTOf9s
- Speech-to-Text & Text-to-Speech
- Conversion
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:hlinkClick r:id="rId7"/></a:rPr><a:t>https://www.youtube.com/watch?v=7uFycTtMwdk
- Text-to-Speech Explained: The Future of Digital Interactions
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:hlinkClick r:id="rId8"/></a:rPr><a:t>https://www.youtube.com/watch?v=257RtqWDa0Q

### Slide 16
- Additional
- learning
- R
- esources
- Microsoft Learn — Azure AI Speech Documentation
- https://learn.microsoft.com/en-us/azure/ai-services/speech-service/
- Google Cloud — Text-to-Speech
- https://cloud.google.com/text-to-speech
- AWS — Amazon Transcribe
- https://aws.amazon.com/transcribe/
- AWS — Amazon Polly
- https://aws.amazon.com/polly/
- Mozilla
- Deep Speech
- Project
- https://github.com/mozilla/DeepSpeech
- Hugging Face — Speech Processing Models
- https://huggingface.co/tasks/automatic-speech-recognition

### Slide 17
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 18
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


---
