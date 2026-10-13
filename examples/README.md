# Cue Editor Practice Project

*The Lantern* is an invented 45-second project for exploring Cue Editor without
production files. It includes 17 cues: dialogue, beats, scene headings, displayed
text, shared speakers, a voiceover, and a subtitle-labeling candidate.

The video is a simple illustrated room with a quiet tone. Its dialogue and actor
names are invented; the text is not a transcription of that tone. One dialogue
cue deliberately contains a number and a blank visibility label so Full Review
has something to inspect.

## Download

- [The Lantern project](The%20Lantern.gooddl-cue-project).
- [Practice video](tutorial.mp4).
- [Practice cue CSV (Comma-Separated Values)](tutorial.csv).

Open each file link and use GitHub's **Download raw file** control to save it.
Keep the original file extensions. You can also choose **Code → Download ZIP**
on the repository's main page to download all documentation and practice files.

## Open the practice project

1. Open Cue Editor and choose **File → Open Project**.
2. Select `The Lantern.gooddl-cue-project`.
3. Choose **File → Add Project Video…** and select `tutorial.mp4`.
4. Confirm a frame rate of **24** and a timeline origin of **01:00:00:00**.
   The practice project's timing already uses this origin.
   To match the screenshots, set **Settings → Layout…** to Beat and Slug on row
   1, Dialog on row 2, and On-screen text on row 3.
5. Select cue 0004 to see an italic word and multiple categories. Try editing a
   field, playing the cue with **Shift+Space**, and undoing the change.
6. Open **Review → Full Review** to inspect cue 0007, or **Review → QC
   (Quality Control) review** to visit every cue.
7. Choose **Utilities → Label Subtitles** to inspect the speaker suggestion for
   cue 0006.
8. Save a copy before trying larger changes. Export to a folder of your choice.

The project opens on a virtual timeline before you add the video. The Cue Editor
project and the cue CSV are alternative starting points: do not append the CSV
to the already populated project unless you intentionally want duplicate cues.

This example does not include production episode support or an external GoodDL
transcription engine. Automatic On/Off labeling and re-transcription need their
own prepared inputs, as explained in the [user guide](../docs/user-guide.md).
