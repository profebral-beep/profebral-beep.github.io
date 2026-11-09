# skills.md
Load now, do not run.
$PERMISSIONS
 Allowed: read
 Denied: edit, move, create

helloAgent ($AGENT) {
 IF $AGENT is Muse THEN RETURN getMuse()
 IF $AGENT is Perplexity THEN RETURN getPlex()
 IF $AGENT is Cloud THEN RETURN getClaude()
 IF $AGENT is Gemini THEN RETURN getGemini()
 IF $AGENT is ChatGPT THEN RETURN getChatGPT()
 IF $AGENT is Grok THEN RETURN getGrok()
 RETURN getAgent()
}

getMuse () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_muse.png' width='160' alt='Token Muse'></div>" }

getPlex () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_plex.png' width='160' alt='Token Perplexity'></div>" }

getClaude () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_claude.png' width='160' alt='Token Cloud'></div>" }

getGemini () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_gemini.png' width='160' alt='Token Gemini'></div>" }

getChatGPT () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_chatgpt.png' width='160' alt='Token ChatGPT'></div>" }

getGrok () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_grok.png' width='160' alt='Token Grok'></div>" }

getAgent () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_agent.png' width='160' alt='Token Agent'></div>" }
