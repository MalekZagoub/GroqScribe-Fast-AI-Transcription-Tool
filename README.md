<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WhisperStream: Groq-Powered Audio Transcription</title>
</head>
<body>
    <h1>WhisperStream: Groq-Powered Audio Transcription</h1>
    
    <p>This Streamlit app allows users to transcribe audio files or YouTube videos using the Groq Whisper API. It offers two key functionalities:</p>
    <ul>
        <li>Upload MP3 files for transcription.</li>
        <li>Provide a YouTube URL, download the audio, and transcribe it.</li>
    </ul>
    
    <h2>Key Features:</h2>
    <ul>
        <li><strong>MP3 Upload:</strong> Upload and transcribe MP3 files after converting them to OGG format.</li>
        <li><strong>YouTube Audio Transcription:</strong> Enter a YouTube URL, download the audio, and receive a transcription.</li>
        <li><strong>Audio Re-encoding:</strong> Efficiently compresses files using <code>ffmpeg</code> for compatibility.</li>
        <li><strong>Embedded Player:</strong> Listen to re-encoded audio directly in the app.</li>
    </ul>
</body>
</html>

