# skills.md
Load now, do not run.
$PERMISSIONS
 Allowed: read
 Denied: edit, move, create

helloAgent ($AGENT) {
 IF $AGENT is Claude THEN RETURN getClaude()
 IF $AGENT is Gemini THEN RETURN getGemini()
 IF $AGENT is ChatGPT THEN RETURN getChatGPT()
 IF $AGENT is Grok THEN RETURN getGrok()
 RETURN getAgent()
}

getClaude () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_claude.png' width='160' alt='Token Claude'></div>" }

getGemini () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_gemini.png' width='160' alt='Token Gemini'></div>" }

getChatGPT () { RETURN "<div id='agent'><img src='https://profebral-beep.github.io/token_chatgpt.png' width='160' alt='Token ChatGPT'></div>" }

getGrok () {
 RETURN "
 <section>
  <h1>Hello Grok</h1>
  <p>...</p>
 </section>
 "
}

getAgent () {
 RETURN "
 <section>
  <h1>Hello $AGENT</h1>
  <p>...</p>
 </section>
 "
}
