1. We can run bash commands directly in claude CLI. Why? So that it stores the context of the commands and can help debug later.

- Use Shift+1 (!) to get into bash mode

2. Creating & Activating a virtual environment:

- python -m venv venv
- source venv/Scripts/activate

3. Installing packages:

- pip install -r requirements.txt

4. The ! prefix in Claude Code spawns a new shell each time, so activation never sticks. In a real terminal, one activate is enough.
