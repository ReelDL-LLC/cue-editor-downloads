# Cue Editor Category Reference

The 46 canonical categories available in Cue Editor 2.6.5. A cue may have multiple categories; saved text joins distinct labels with `|`. Choose the canonical suggestion when assigning a category.

**TC (Timecode)** appears in the stored timing-check labels. **SFX (Sound Effects)** appears in the stored sound-effects-overlap label. Labels are identifiers; their exact spelling matters.

[Return to category editing in the user guide](user-guide.md#add-and-remove-categories)

## Assign and interpret categories

In 2.6.5, enter a label in **Add category**, accept its suggestion, and remove a category with its chip’s **×** button. Earlier versions use the categories text field. Automatic categories are reassessed after committed edits. Manual choices retain their applicable review context, but a split or merge can require reassessment.

A label is not proof that an audio classifier ran. Some categories are assigned from text or annotations, some are suggestions, and some require listening or a verified raw/reference comparison. Do not infer a verified negative from a missing label. Review approval does not turn automatic evidence into a verified reference.

## Category meanings

| Display name | Stored label | Meaning |
| --- | --- | --- |
| Quiet | `quiet` | Dialogue whose spoken voice is unusually low in level relative to comparable nearby dialogue. A transcription miss alone is not evidence of quiet delivery. No numerical threshold has been validated. |
| Whisper | `whisper` | Speech delivered with whispered vocal quality, regardless of recording volume. |
| Shout | `shout` | Speech delivered with shouted vocal quality and vocal effort, rather than merely recorded loudly. Preserve the editorial convention of using an exclamation point in place of a terminal period when appropriate. |
| Accent | `accent` | The retained legacy label for speech delivered with a non-United States American accent. This broad label is not a sufficient definition for an accent-specific training experiment. |
| Digital | `digital` | Speech with audible electronic filtering or processing, such as a voice modulator, radio, television, or public-address effect. Clear speech heard through a device does not qualify. |
| Stifled | `stifled` | An utterance abruptly interrupted by another source before completion. End the interrupted text with a hyphen, as in `But I thought-`. |
| Trails Off | `trails_off` | An utterance that gradually stops before completing the thought. End the text with an ellipsis, as in `But I thought...`. |
| Unclear | `unclear` | A human-confirmed unintelligible portion of a cue. Keep as a reference-quality state as well as a compatibility label. Exclude from ordinary speech training and evaluation until the uncertainty is resolved. |
| Review | `review` | A cue requiring unresolved human review, including low-confidence transcription or an uncertain reference. Keep the reason and resolution separately from observable speech categories. |
| Background | `background` | Dialogue from a background source that is not pertinent to the plot. This is an editorial relevance judgment, distinct from low volume and competing background conversation. |
| Laughing | `laughing` | Laughter affects the delivery of the words themselves. A separate laugh before, after, or between otherwise ordinary speech does not qualify. |
| Nonverbal | `nonverbal` | A cue containing a recognized nonverbal event annotation, such as `(sighs)`, including equivalent recognized square-bracket annotations. This can coexist with spoken words. |
| Nonverbal Easy | `nonverbal_easy` | A readily identifiable vocal response written as words rather than a parenthetical, such as `Mm.`, `Mm-hmm.`, or `Uh-huh.`. These responses remain speech targets when accurately transcribed. |
| Song Recording | `song_recording` | Lyrics from a musical performance heard on a recording. |
| Singing | `singing` | The target vocal contains sung words, including casual singing and musical performances. Recorded performance context can also be identified with `song_recording`. |
| Overlap | `overlap` | A summary label for concurrent dialogue or competing sound meeting one of the specific overlap definitions. Retain existing generic labels when the subtype is unknown. |
| Dialog Overlap | `dialog-overlap` | Two distinct sources produce audible speech simultaneously within the cue. Concurrent speech does not itself establish that the reference is unusable. |
| Sound Effects Overlap | `sfx-overlap` | Sound effects compete with and obscure the target speech, such as construction or explosions. |
| Music Overlap | `music-overlap` | Music competes with the target voice and makes the words harder to hear. The words can remain intelligible. |
| Walla Overlap | `walla-overlap` | Indistinct background conversation competes with and obscures the target speech. |
| Editor Cheat | `editor_cheat` | An editorial splice makes a character appear to say something different from the original utterance. The reference must still represent words audible in the selected clip. |
| Scene Change | `scene_change` | One continuing utterance spans a scene boundary or slug line. |
| Slang | `slang` | A colloquial word or an expression used with a colloquial meaning, such as `bet` meaning “all right” or “agreed”, or `hoochies`. A shortened pronunciation retaining the ordinary meaning, such as `knockin’` for `knocking`, is an `abbreviation`, not slang on that basis alone. |
| Number | `number` | Spoken text contains a quantity, date, time, monetary amount, ordinal, or numeric identifier, including numbers written as words. |
| Acronym | `acronym` | A sequence of two or more uppercase letters in dialogue, either contiguous or separated by periods. This review category includes letter-by-letter initialisms and fully capitalized words; a known expansion or word-like pronunciation is not required. |
| Contraction | `contraction` | A conventional grammatical contraction, such as `don't` or `we're`. Possessives do not qualify. |
| Abbreviation | `abbreviation` | A shortened lexical form or letter-by-letter initialism with a known intended expansion. Grammatical contractions use their own label. Uppercase initialisms also receive `acronym` under the review convention. This includes pronunciation elisions such as `knockin’` → `knocking`, `goin’` → `going`, and `nothin’` → `nothing`. For example, `'cuz` qualifies only when context establishes the intended full word. |
| Question | `question` | A cue in which the speaker asks a question. A question mark in reviewed dialogue is the text-based assignment signal; a question mark in an uncertain automatic transcript remains provisional. |
| Proper Name | `proper_name` | Spoken text names a particular person, place, organization, brand, or other named entity. |
| Perfect | `perfect` | All four raw/reference checks pass: `correct-text`, `correct-speaker`, `correct-tc-length`, and `correct-tc`. |
| Imitation | `imitation` | A character imitates or does an impression of another character's, celebrity's, or creature's voice. |
| Stammer | `stammer` | A cue contains a hesitant repetition or restart of a sound, word, or short phrase, such as "That's- that's not fair." or "I, I get that, I do." |
| Pause | `pause` | A character takes a long pause between their lines or phrases of dialogue, often denoted by an ellipsis. |
| Hesitation | `hesitation` | A cue contains a spoken filler used as a filled pause while the character hesitates or plans their next words, such as "Um, let me think." |
| Slurred | `slurred` | A cue contains slurred speech, with words or speech sounds running together and reduced clarity of articulation. |
| Profanity | `profanity` | A cue contains one or more spoken curse words or swear words. |
| Discourse Marker | `discourse_marker` | A dialogue cue contains a sentence beginning with a conversational word or short phrase, such as “Look, I'm not...”, “Hey, why do...”, or “You know, that's true.” The sentence can occur anywhere in the cue. |
| Main Title | `main-title` | A cue contains the title of its own show, including a spoken title or an onscreen title. |
| Symbol | `symbol` | A spoken expression was originally rendered with a symbol in the matching raw As Broadcast Script, whether it remains symbolic or is now written out: `A+` → `A plus`, `#gay` → `Hashtag: gay`, or `100%` → `One-hundred percent`. |
| Air Quote | `air-quote` | Words or phrases appear in quotation marks within a sentence without a comma introducing them, such as `she spotted your "discreet" tail`. |
| Quote | `quote` | A character quotes someone or something, as in `He said, “Dead men tell no tales.” Does that mean anything to you?` |
| Emphasis | `emphasis` | The character puts extra vocal emphasis on one or more words, which are marked in italics in the transcript. |
| Correct Text | `correct-text` | The raw dialogue transcript exactly matches the reviewed reference text, including punctuation, capitalization, and whitespace. |
| Correct Speaker | `correct-speaker` | The raw dialogue speaker exactly matches the speaker in the reviewed reference. |
| Correct Timecode Length | `correct-tc-length` | The raw cue duration matches the reviewed reference duration, calculated from valid start and end timecodes in frames. |
| Correct Timecodes | `correct-tc` | Both the raw start timecode and raw end timecode match the reviewed reference boundaries at frame precision. |

## Reference checks

The four `correct-` labels compare the original raw cue with a reviewed reference: text, speaker, duration, and both timing boundaries. `perfect` requires all four checks to pass. Without a supported raw/reference relationship, these checks are unassessed. An ordinary cue approval is not an accuracy measurement.

## Legacy labels

Older overlap labels may be normalized to `dialog-overlap`, `sfx-overlap`, `music-overlap`, and `walla-overlap`. Existing generic `overlap` can remain when the subtype is unknown. A legacy `Song` or `song` value needs listening review to choose `singing` and/or `song_recording`; changing case cannot establish the subtype.
