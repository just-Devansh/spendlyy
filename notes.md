1. We can run bash commands directly in claude CLI. Why? So that it stores the context of the commands and can help debug later.

- Use Shift+1 (!) to get into bash mode

2. Creating & Activating a virtual environment:

- python -m venv venv
- source venv/Scripts/activate

3. Installing packages:

- pip install -r requirements.txt

4. The ! prefix in Claude Code spawns a new shell each time, so activation never sticks. In a real terminal, one activate is enough.

5. SLASH Commands:
   - shortcuts you type inside a Claude Code session, which trigger a specific predefined action - without writing a full prompt
   - a. built-in b. custom

6. Session: A session is one conversation with Claude Code

- claude --> /exit
- it has a unique ID and captures the full message history
- sessions are saved automatically to ~/.claude/projects/ and can be resumed at any time

7. To resume a session: claude -r
8. To switch to a different session mid-session: /resume
9. Good Practices related to sessions:
   - One session = One task
   - Name your session immediately (/rename [name])
   - Commit frequently within a session
   - Use /btw for quick questions (avoids polluting context)
   - Export a session before a big refactor (/export file.md)

10. Other Slash Commands
    a. /logout (successfully logout from your Anthropic account)
    b. /usage (daily and weekly usage %)
    c. /stats (usage statistics and user behaviour)
    d. /insights (generates an HTML insight based on how we're using Claude Code. What we're doing right/wrong and other suggestions.)
    e. /config (modify Claude Code configurations)
    f. /permissions (of tools that Claude Code uses to do it's thing. ex: Bash[git init], WebSearch, etc.)
    g. /theme
    h. /voice (toggles voice-mode)

11. Models:

- Opus: most powerful but most expensive
- Sonnet: default for most users. all-rounder
- Haiku: fastest and cheapest. used for simple tasks

12. Pro Tip: Use Opus for the planning phase then switch to Sonnet (/model)

13. Use @ (mention to direct claude to specific files and make changes
