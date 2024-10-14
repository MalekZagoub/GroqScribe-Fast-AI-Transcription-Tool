<h1>WhisperStream: Groq-Powered Audio Transcription</h1>

![image](https://github.com/user-attachments/assets/d32b4910-6d17-46d6-ae99-5f3496abb94a)

<p>This Streamlit-based app allows users to transcribe audio files or YouTube videos using the Groq Whisper API. It provides two main functionalities:</p>
<ul>
  <li>Upload an MP3 file for transcription.</li>
  <li>Input a YouTube URL, download the audio, and transcribe it.</li>
</ul>

<h2>Features</h2>
<ul>
  <li><strong>Audio Upload</strong>: Upload any MP3 file, re-encode it to OGG format to reduce file size, and transcribe it using the Groq Whisper API.</li>
  <li><strong>YouTube Audio Download</strong>: Provide a YouTube link, download the audio, re-encode it to OGG, and get a transcription.</li>
  <li><strong>Re-encoding</strong>: Uses <code>ffmpeg</code> to re-encode MP3 files to the Opus codec in OGG format, ensuring compatibility with Whisper's input limits (maximum 25MB).</li>
  <li><strong>Audio Embedding</strong>: After re-encoding, the audio file is embedded in the Streamlit app with a player for users to listen to the audio directly.</li>
</ul>

<h2>Technologies Used</h2>
<ul>
  <li><strong>Streamlit</strong>: Used for building the web interface.</li>
  <li><strong>yt-dlp</strong>: To download YouTube videos and extract audio.</li>
  <li><strong>pydub</strong>: Audio processing library.</li>
  <li><strong>ffmpeg</strong>: Used for re-encoding the audio into OGG format. This compresses the audio significantly while retaining quality suitable for transcription.</li>
  <li><strong>Groq Whisper API</strong>: Used for transcribing the audio.</li>
  <li><strong>Python</strong>: Core programming language for the app.</li>
</ul>

<h2>Prerequisites</h2>
<p>Before you begin, ensure you have the following installed:</p>
<ul>
  <li>Python 3.10 or higher</li>
  <li><code>ffmpeg</code> (ensure it’s in your system's PATH)</li>
  <li>Necessary Python dependencies (installed using <code>requirements.txt</code>)</li>
</ul>

<h2>Installation</h2>
<ol>
  <li>Clone this repository:</li>
  <pre><code>git clone https://github.com/Vinay9911/Groq-Whisper-Fast-Transcription-App.git</code></pre>
  
  <li>Navigate to the project directory:</li>
  <pre><code>cd groq-whisper-fast-transcription-app</code></pre>
  
  <li>Install the required Python packages:</li>
  <pre><code>pip install -r requirements.txt</code></pre>
  
  <li>Ensure <code>ffmpeg</code> is installed on your machine and available in your system's PATH.</li>
  
  <li>Create a <code>.env</code> file in the root directory with the following contents:</li>
  <pre><code>GROQ_API_KEY=your_groq_api_key</code></pre>
  Replace <code>your_groq_api_key</code> with your actual Groq Whisper API key.
</ol>

<h2>Usage</h2>
<ol>
  <li>Run the Streamlit app:</li>
  <pre><code>streamlit run transcript.py</code></pre>

  <li>The app will open in your default web browser. You can also access it at <code>http://localhost:8501</code>.</li>

  <li>Transcription Options:
    <ul>
      <li><strong>Tab 1 - Upload Audio</strong>: Upload an MP3 file, which will be re-encoded and then transcribed using Groq Whisper.</li>
      <li><strong>Tab 2 - YouTube to Audio</strong>: Enter a YouTube video URL, download the audio, and get a transcription.</li>
    </ul>
  </li>
</ol>

<h2>Notes</h2>
<ul>
  <li>The Groq Whisper API can transcribe long audio files, but re-encoding is necessary to reduce file size for optimal performance.</li>
  <li>Ensure you have a


