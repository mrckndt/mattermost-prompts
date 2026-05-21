# mattermost-prompts

## Constraints

### techsupport-agent.md
Maximum 16,383 runes (Unicode code points). Check after every edit:
```
python3 -c "print(len(open('techsupport-agent.md').read()))"
```
If over, trim prose in the agent preamble or operating environment section before touching skill logic.
