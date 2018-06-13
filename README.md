# Git screencast

As of now, Git screencast is about 14 hours of high quality educational material about Git.

It's here: http://learn.javascript.ru/screencast/git, but we look forward to put it to a separate domain, as it's not related to Javascript.

It is in Russian, because that language is most convenient for me, and I can ensure good language and pronunciation.

**Here we translate it to English, and that will be the base version for other translators, Chinese and other languages.**

The translation process can be split into 4 parts.

## 1. Make subtitles from the Russian version.

Requirements: understanding Russian, git knowledge.

E.g. for the 1st video:

- Add label "In Progress: Russian srt", so that other people know you're working on it.
- Go to video at (https://www.youtube.com/playlist?list=PLDyvV36pndZHkDRik6kKF6gSb0N0W995h)[Youtube].
- Add subtitles following <https://support.google.com/youtube/answer/6054623?hl=en>.
- Download the subtitles and make PR them.

If you commit it, add label "Need translation", so that other people know that the srt is complete.

P.S. That "srt" file is not only for translation, it's good on its own. Allows to enable subtitles on youtube.


## 2. Translate subtitles

Requirements: understanding Russian, very good English.

- Find an issue labelled with "Need translation", e.g. `01-01-intro`.
- Relabel it as "In Progress: translation", to let others know that you're making it.
- Copy `01-01-intro/01-01-intro.ru.srt` to `01-01-intro/01-01-intro.en.srt`.
- Translate the phrases, without changing any timestamps. We'll fix the timestamps after voicing the translation.
- Make a PR (not commit).
- Relabel it as "Need review".

## 3. Review translations

Requirements: native English, git knowledge.

- Look at PRs, review the translation to ensure good English and good git.
- Merge PR
- Label the corresponding issue with `Need Voice`.

## 4. Voice the screencast

Requirements: native English, good diction, external Mic for quality sound.

Guess, there will be a single person to be the narrator of the English screencast.

For simple cases, one can just voice over the existing screencast, without any video editing,
so that we replace the audio afterwards, and that's it.

If the translated speech does not lay over well, the screencast can be edited, video frames can be made longer/shorter. Presentations may be adjusted.

You can edit the screencast on Mac. Or you can make the voice over, and then @iliakan can edit the screencast to correspond to the speech.

The final variant goes to `01-01-intro/01-01-intro.en.flac` (or maybe mp4 with high bitrate?).

Then we'll adjust the English subtitles for the timing.
