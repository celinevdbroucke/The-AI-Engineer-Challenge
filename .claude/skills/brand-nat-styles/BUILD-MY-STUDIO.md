# Installer instructions for Claude Code
When asked to install this archive, install Brand Nat Style Pack.zip first, then follow Build My Studio.md. Read the style pack README and SKILL.md before installation. Ask whether to use project or personal skills. Preserve existing files: reuse identical skills, ask before replacing different versions. Verify the installed styles.md and guide contain 105 style codes. Use the installed skill location for my-studio. The bonus file is the original prompt: execute its text box after installing the styles; do not ask the customer to paste it again. Ask before system-wide dependencies. Do not invent preferences, render without a requested source video, or claim setup complete before the required steps finish.

# Build Your Own Studio

1. Install the 105 styles first.
2. Copy everything in the box below and paste it into Claude Code.

```text
Set up my own video editing studio in Claude Code, on top of my 105 styles.

1. Find the 105 styles skill (usually in ~/.claude/skills, or in this project's .claude/skills). It's the one with a styles.md and a style guide. If it isn't there, tell me to install it first and stop. If there's more than one, ask me which to use.

2. Make a skill called my-studio in the same skills folder as the 105 styles skill. Description: use whenever I edit a video, give a note on an edit, or approve a video. Use the 105 styles skill when editing and let my saved preferences guide the choices. If my-studio already exists, keep my files.

3. Keep two files in it:
   - MY-STYLE.md: my look (captions, colours, pacing) and anything I never want.
   - NOTES.md: every note I give.

4. Check ffmpeg is set up, the way the 105 styles skill does it. Then find my style once: ask me for 1 to 3 video files I love, or my own videos. If I have none, help me pick styles from the 105 style guide. Look at frames from the videos and save what I like to MY-STYLE.md. Learn the style, don't copy the video.

5. Every edit: read both files first and follow them. Read them again right before you render, so nothing gets forgotten halfway through. Then check the finished video against every rule, one by one, and label each check:
   - Measured: you measured it on the actual video file (words per line, gaps, how long nothing moves).
   - Visually reviewed: you looked at frames from the actual video.
   - Unverified: you couldn't check it on the video. Only the plan or an estimate says it's fine.
   Never say a check passed if it was only based on the plan or an estimate. Fix anything that fails before you show me, then give me the list with its labels.

6. Every note: save it in NOTES.md the moment I give it, before you start fixing anything. Don't wait until the end. If I've said it before, add it to MY-STYLE.md as a rule and tell me "You've said this before, so it's now a rule." When I approve a video, save what worked to MY-STYLE.md.

7. Make sure every new chat uses my-studio. Add this line to the right CLAUDE.md: "When I send a video, give a note on an edit, or approve one, use the my-studio skill first."
   - If my skills are personal (in ~/.claude/skills), use ~/.claude/CLAUDE.md.
   - If my skills are in this project (in .claude/skills), use CLAUDE.md in this project's main folder.
   Keep everything already in that file. Only add the line at the end, and don't add it twice. If the file doesn't exist, make it with just that line.

When it's done, say: "Your studio is ready. Start a new chat (in this same project if your skills live there) and send me a video."
```
