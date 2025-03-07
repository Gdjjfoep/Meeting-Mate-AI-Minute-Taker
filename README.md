Overview of the "Meeting Mate: AI Minute Taker" Application
"Meeting Mate: AI Minute Taker" is a desktop application designed to streamline the process of taking meeting minutes by utilizing AI-driven transcription and summarization features. The primary task of this application is to record spoken conversations during virtual meetings and generate accurate, real-time transcriptions, which can then be summarized into key points for easy reference.

Key features include:
1.Live Transcription: Using Deepgram's API, the application captures live audio from virtual meetings and transcribes it in real time. The transcription is displayed in a dedicated highlights area as the conversation progresses.
2.Summarization: Once the transcription is complete, the user can generate a concise summary of the meeting using natural language processing techniques (LSA or TextRank summarization methods) to extract key points.
3.Meeting Integration: The app supports integrating virtual meetings by allowing the user to input a meeting URL, such as for Jitsi meetings, and join directly in the embedded meeting window.
4.Exporting Transcripts: After the meeting ends, the transcript can be exported as a text file for further use or archiving.
5.User-Friendly Interface: The application provides an intuitive interface with clear buttons for starting and stopping transcription, summarizing the meeting, and exporting the transcript, along with a live meeting screen to watch and interact with the virtual meeting.

The overall goal of "Meeting Mate" is to reduce the time and effort involved in manually taking minutes, making meetings more efficient and productive for all participants.

------------------------------------------------------------------------------------------------------------------------------------------

Future Goal:
As this is an early version of the code, it currently depends on a virtual audio cable to loop the audio. For this purpose, I have used the VB Cable and set it as the default device in both the recording and playback tabs. However, the drawback of this approach is that the user will be unable to hear or speak, as the VB Cable is dedicated to handling the audio, while other participants who aren’t using it can still communicate normally.

Since I’m working with a low-end device, I’ve opted for a lightweight summarization module to handle the summary functionality efficiently without taxing system resources. However, if you wish to scale the application or move to a cloud-based solution, you could implement models like GPT-2 (which is open-source) or use other AI APIs for more advanced summarization capabilities.

Looking ahead, I plan to enhance the system by developing a custom server for Jitsi Meet. This would provide us with direct access to the audio stream, allowing us to seamlessly integrate our transcription module powered by Deepgram.

