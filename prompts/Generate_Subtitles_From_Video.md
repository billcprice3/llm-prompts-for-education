# Generating Subtitles from a Video

This guide features a powerful workflow I experimented with in September 2025 for creating accurate, accessible video captions using an open-source tool that can be a valuable asset for any educator working with digital media: [Buzz Captions](https://buzzcaptions.com/).

### A Free Solution for High-Quality Captions

Educators who create or use video content are often faced with the poor quality of auto-generated captions on platforms like YouTube. These captions can be so inaccurate that they are unsuitable for classroom use, creating an accessibility barrier for students.

I recently encountered this issue when preparing a film trailer for a listening comprehension activity. The platform's default captions were not usable. As an alternative, I tried out the open-source program [**Buzz Captions**](https://buzzcaptions.com/) to process the video file locally. Using the `medium` Whisper model, the program generated a nearly-perfect transcript and a ready-to-use `.srt` subtitle file in under a minute. The result was a dramatic improvement in quality over the automatically generated YouTube version of the subtitles.

This workflow is a strong choice for educators who need to produce accurate captions while working entirely offline, thereby keeping all data private and secure on their own computer. It relies on free, open-source tools while offering a professional-grade alternative to paid, proprietary services.

## Quick Start Guide

1.  **Download and Install Buzz.**
    
    -   Navigate to the [Buzz GitHub Releases page](https://github.com/chidiwilliams/buzz/releases).
        
    -   Download the installer for your operating system (macOS, Windows, or Linux).
        
2.  **Prepare Your Media File.**
    
    -   Have your video or audio file (e.g., `.mp4`, `.mp3`) saved locally on your computer.
        
3.  **Run the Transcription.**
    
    -   Open the Buzz application.
        
    -   Drag and drop your media file into the main window.
        
    -   In the pop-up window, confirm your settings. For a strong balance of accuracy and performance, I recommend selecting the `Whisper (Medium)` model.
        
    -   Click `Run` and allow the program to process the file.
        
4.  **Export the Caption File.**
    
    -   Once the status reads `Completed`, double-click the task to open the transcript viewer.
        
    -   Use the `Export` button to save the transcript. For video subtitles, the **`.srt`** format is standard.
  
    -   If your video file is named `videofilename.mkv`, you should name your subtitle filename something like `videofilename.en.srt`, where the first part of the filename is **identical** to the video filename; then a dot; then a [2- or 3-character ISO language code](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) such as `en` for English or `fr` for French, etc.; then `.srt`.
  
5.  **Playing your Video with Captions**

   -   Make sure your video file and subtitle file (`.srt`) are in the same directory and named correctly (see part 4 above).
   
   -   Most modern video player programs such as **[VLC](https://www.videolan.org/vlc/)** will automatically associate the subtitle file with the video file when you open it. You may need to go to `Subtitles` > `Subtitle Track...` in the VLC interface to toggle the visiblility of the subtitle track on-screen.

6.  **Modifying the Subtitles**

   - If your subtitles aren't quite perfect, you can open your `SRT` file in any simple text editing program such as `Notepad` or `TextEdit` and change any mistakes by hand.

## The Underlying Technology: Buzz + Whisper

This workflow's effectiveness comes from the combination of two distinct open-source projects. **[OpenAI Whisper](https://openai.com/index/whisper/)** is the core technology. It’s a state-of-the-art speech recognition model known for its high accuracy on a wide range of audio.

**[Buzz Captions](https://buzzcaptions.com/)** is the graphical user interface (GUI) that makes the Whisper model accessible to the average user. It provides a usable front-end interface for the complex underlying language model, allowing you to run powerful transcriptions locally without writing code. This offline approach is a key advantage, as it ensures privacy and gives the user full control over their data and workflow, a practice consistent with the principle of digital sovereignty. (I like knowing that once I have a tool, it’s mine forever, and that a tech company can’t delete the tool from my device or remove my access later!)

The drafting of this writeup was accelerated with AI assistance, but recounts my genuine experience and opinion.
