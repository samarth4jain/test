# test


flowchart TD

    A[Teacher Input<br/>Voice / Photo / Text] --> B{Cloud Functions}
    B --> C1[Gemini Model<br/>Text/Image Generation]
    B --> C2[Vertex AI STT / TTS<br/>Speech Processing]
    C1 --> D1[Generated Content]
    C2 --> D2[Transcript / Answer]
    D1 --> E1[Stored in Firebase]
    D2 --> E1
    E1 --> F[Displayed / Played Back in App]
