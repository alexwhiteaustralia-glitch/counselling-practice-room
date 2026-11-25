# Setup card

When "practice room" calls for the setup card and the chat can show an interactive widget, render the form below exactly as it is (it uses the widget's built-in form styles; no script needed). Defaults are pre-selected. Don't rebuild, trim or restyle it. If the chat can't show a widget, use the numbered-list fallback described in `SKILL.md`.

```html
<h2 class="sr-only">Practice Room setup card with session settings and defaults selected.</h2>
<form class="elicit">
  <div class="elicit-header">
    <span>Practice room details</span>
  </div>
  <div class="elicit-body">
    <div class="elicit-group">
      <label class="elicit-question">What would you like to do?</label>
      <div class="elicit-pills" data-name="mode" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Session" aria-pressed="true" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-armchair" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Session</span><br><span style="font-size:11px; color:var(--text-muted)">10 min, one client, everyday</span></span></button>
        <button type="button" class="elicit-pill" data-value="Rehearsal" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-microphone" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Rehearsal</span><br><span style="font-size:11px; color:var(--text-muted)">Full arc, before an assessment</span></span></button>
        <button type="button" class="elicit-pill" data-value="Deep session" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-stack-2" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Deep session</span><br><span style="font-size:11px; color:var(--text-muted)">20 min, follow what's underneath</span></span></button>
        <button type="button" class="elicit-pill" data-value="Replay" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-rewind-backward-10" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Replay</span><br><span style="font-size:11px; color:var(--text-muted)">Redo a real session from its transcript</span></span></button>
        <button type="button" class="elicit-pill" data-value="Drill" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-repeat" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Drill</span><br><span style="font-size:11px; color:var(--text-muted)">Five reps on one skill</span></span></button>
        <button type="button" class="elicit-pill" data-value="Edge drill" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-target" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Edge drill</span><br><span style="font-size:11px; color:var(--text-muted)">Six reps on your habits</span></span></button>
        <button type="button" class="elicit-pill" data-value="Warm-up" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-flame" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Warm-up</span><br><span style="font-size:11px; color:var(--text-muted)">Quick mixed reps</span></span></button>
        <button type="button" class="elicit-pill" data-value="Casebook" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-users" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Casebook</span><br><span style="font-size:11px; color:var(--text-muted)">Your nine ongoing clients</span></span></button>
        <button type="button" class="elicit-pill" data-value="Favourites drill" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-star" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Favourites drill</span><br><span style="font-size:11px; color:var(--text-muted)">Reps from your shortlist</span></span></button>
        <button type="button" class="elicit-pill" data-value="More" data-other style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:150px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-dots" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">More</span><br><span style="font-size:11px; color:var(--text-muted)">Ladder, close, repair...</span></span></button>
      </div>
      <input type="text" class="elicit-other" data-for="mode" placeholder="e.g. ladder drill, close drill, stage spot, or 'options'" hidden>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Which skill? (skip for an edge drill, replay or casebook)</label>
      <div class="elicit-pills" data-name="skill" data-multi="false">
        <button type="button" class="elicit-pill" data-value="All skills" aria-pressed="true">All skills</button>
        <button type="button" class="elicit-pill" data-value="Opening and goal setting">Opening</button>
        <button type="button" class="elicit-pill" data-value="Listening and attending">Listening</button>
        <button type="button" class="elicit-pill" data-value="Paraphrasing, restating and summarising">Paraphrase and summarise</button>
        <button type="button" class="elicit-pill" data-value="Open questions">Open questions</button>
        <button type="button" class="elicit-pill" data-value="Reflecting feeling">Reflecting feeling</button>
        <button type="button" class="elicit-pill" data-value="Advanced empathy">Advanced empathy</button>
        <button type="button" class="elicit-pill" data-value="Use of silence">Silence</button>
        <button type="button" class="elicit-pill" data-value="Focusing">Focusing</button>
        <button type="button" class="elicit-pill" data-value="Therapeutic presence">Presence</button>
        <button type="button" class="elicit-pill" data-value="Immediacy">Immediacy</button>
        <button type="button" class="elicit-pill" data-value="Confronting">Confronting</button>
        <button type="button" class="elicit-pill" data-value="Reflection of meaning">Meaning</button>
        <button type="button" class="elicit-pill" data-value="Working with ambivalence">Ambivalence</button>
        <button type="button" class="elicit-pill" data-value="Culture and worldview">Culture</button>
        <button type="button" class="elicit-pill" data-value="Self-criticism and self-destructive processes">Self-criticism</button>
        <button type="button" class="elicit-pill" data-value="Unpacking and triggers">Unpacking</button>
        <button type="button" class="elicit-pill" data-value="Re-experiencing and sequencing">Re-experiencing</button>
        <button type="button" class="elicit-pill" data-value="Polarities">Polarities</button>
        <button type="button" class="elicit-pill" data-value="Rupture and repair">Rupture and repair</button>
        <button type="button" class="elicit-pill" data-value="Ending a session">Ending</button>
        <button type="button" class="elicit-pill" data-value="Integration">Integration</button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">How long will you run it? (you keep the timer)</label>
      <div class="elicit-pills" data-name="length" data-multi="false">
        <button type="button" class="elicit-pill" data-value="5 min">5 min</button>
        <button type="button" class="elicit-pill" data-value="10 min" aria-pressed="true">10 min</button>
        <button type="button" class="elicit-pill" data-value="20 min">20 min</button>
        <button type="button" class="elicit-pill" data-value="30 min">30 min</button>
        <button type="button" class="elicit-pill" data-value="40 min">40 min</button>
        <button type="button" class="elicit-pill" data-value="50 min">50 min</button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Observer reminders during the session?</label>
      <div class="elicit-pills" data-name="nudges" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Skill flags" aria-pressed="true" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:140px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-flag" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">At key moments</span><br><span style="font-size:11px; color:var(--text-muted)">Only the bigger misses</span></span></button>
        <button type="button" class="elicit-pill" data-value="On request" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:140px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-hand-stop" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Only on request</span><br><span style="font-size:11px; color:var(--text-muted)">Say "nudge" for one</span></span></button>
        <button type="button" class="elicit-pill" data-value="Off" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:140px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-volume-off" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Off</span><br><span style="font-size:11px; color:var(--text-muted)">Save it for the debrief</span></span></button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Client's gender?</label>
      <div class="elicit-pills" data-name="client_gender" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Any" aria-pressed="true">Any</button>
        <button type="button" class="elicit-pill" data-value="Woman">Woman</button>
        <button type="button" class="elicit-pill" data-value="Man">Man</button>
        <button type="button" class="elicit-pill" data-value="Non-binary">Non-binary</button>
        <button type="button" class="elicit-pill" data-value="Trans woman">Trans woman</button>
        <button type="button" class="elicit-pill" data-value="Trans man">Trans man</button>
        <button type="button" class="elicit-pill" data-value="Genderfluid">Genderfluid</button>
        <button type="button" class="elicit-pill" data-value="Agender">Agender</button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">How old are they?</label>
      <div class="elicit-pills" data-name="client_age" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Any">Any</button>
        <button type="button" class="elicit-pill" data-value="18 to 24">18–24</button>
        <button type="button" class="elicit-pill" data-value="25 to 34">25–34</button>
        <button type="button" class="elicit-pill" data-value="35 to 44">35–44</button>
        <button type="button" class="elicit-pill" data-value="45 to 54" aria-pressed="true">45–54</button>
        <button type="button" class="elicit-pill" data-value="55 to 64">55–64</button>
        <button type="button" class="elicit-pill" data-value="65 to 74">65–74</button>
        <button type="button" class="elicit-pill" data-value="75 and over">75+</button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">How open are they?</label>
      <div class="elicit-pills" data-name="attitude" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Open" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:140px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-door" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Open</span><br><span style="font-size:11px; color:var(--text-muted)">Names feelings easily</span></span></button>
        <button type="button" class="elicit-pill" data-value="Medium" aria-pressed="true" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:140px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-door-enter" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Medium</span><br><span style="font-size:11px; color:var(--text-muted)">Opens to accurate reflection</span></span></button>
        <button type="button" class="elicit-pill" data-value="Guarded" style="border-radius:12px; padding:12px 14px; display:flex; gap:10px; align-items:flex-start; text-align:left; min-width:140px; box-shadow:0 1px 2px rgba(0,0,0,0.04)"><i class="ti ti-lock" style="font-size:18px" aria-hidden="true"></i><span><span style="font-size:13px; font-weight:500">Guarded</span><br><span style="font-size:11px; color:var(--text-muted)">Short answers, deflects</span></span></button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Any particular style? (optional)</label>
      <div class="elicit-pills" data-name="client_style" data-multi="false">
        <button type="button" class="elicit-pill" data-value="None" aria-pressed="true">None</button>
        <button type="button" class="elicit-pill" data-value="Deflects with humour">Deflects with humour</button>
        <button type="button" class="elicit-pill" data-value="Intellectualises">Intellectualises</button>
        <button type="button" class="elicit-pill" data-value="Goes quiet">Goes quiet</button>
        <button type="button" class="elicit-pill" data-value="Gets briefly tearful">Briefly tearful</button>
        <button type="button" class="elicit-pill" data-value="Seeks approval">Seeks approval</button>
        <button type="button" class="elicit-pill" data-value="Agrees politely">Agrees politely</button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">How weighty is what they bring?</label>
      <div class="elicit-pills" data-name="depth" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Light">Light</button>
        <button type="button" class="elicit-pill" data-value="Moderate" aria-pressed="true">Moderate</button>
        <button type="button" class="elicit-pill" data-value="Weighty">Weighty</button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Where are you in the work together?</label>
      <div class="elicit-pills" data-name="phase" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Suits the mode" aria-pressed="true">Suits the mode</button>
        <button type="button" class="elicit-pill" data-value="First session">First session</button>
        <button type="button" class="elicit-pill" data-value="Middle phase">Middle phase</button>
        <button type="button" class="elicit-pill" data-value="Ending phase">Ending phase</button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">What are they coming in with?</label>
      <div class="elicit-pills" data-name="theme" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Surprise me" aria-pressed="true">Surprise me</button>
        <button type="button" class="elicit-pill" data-value="Give me three options">Give me three options</button>
        <button type="button" class="elicit-pill" data-value="Going back to study">Going back to study</button>
        <button type="button" class="elicit-pill" data-value="A housemate over shared space">Housemate tension</button>
        <button type="button" class="elicit-pill" data-value="A close friend moving interstate">Friend moving interstate</button>
        <button type="button" class="elicit-pill" data-value="Can't switch off from work">Can't switch off</button>
        <button type="button" class="elicit-pill" data-value="A conversation with a manager">Talking to a manager</button>
        <button type="button" class="elicit-pill" data-value="An adult child moving out">Adult child moving out</button>
        <button type="button" class="elicit-pill" data-value="A stalled creative project">Stalled creative project</button>
        <button type="button" class="elicit-pill" data-value="A parent needing more help">Parent needing help</button>
        <button type="button" class="elicit-pill" data-value="Drifting from old friends">Drifting from friends</button>
        <button type="button" class="elicit-pill" data-value="A career change">Career change</button>
        <button type="button" class="elicit-pill" data-value="Replaying a snap at a partner">Snapped at a partner</button>
        <button type="button" class="elicit-pill" data-value="Something of my own" data-other>Something of my own</button>
      </div>
      <input type="text" class="elicit-other" data-for="theme" placeholder="Describe the theme" hidden>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Their background?</label>
      <div class="elicit-pills" data-name="background" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Varied" aria-pressed="true">Varied</button>
        <button type="button" class="elicit-pill" data-value="My choice" data-other>I'll name one</button>
      </div>
      <input type="text" class="elicit-other" data-for="background" placeholder="Which background?" hidden>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">Arrive first?</label>
      <div class="elicit-pills" data-name="arrive" data-multi="false">
        <button type="button" class="elicit-pill" data-value="On" aria-pressed="true">On</button>
        <button type="button" class="elicit-pill" data-value="Off">Off</button>
      </div>
    </div>
    <div class="elicit-group">
      <label class="elicit-question">How much debrief?</label>
      <div class="elicit-pills" data-name="debrief" data-multi="false">
        <button type="button" class="elicit-pill" data-value="Full" aria-pressed="true">Full</button>
        <button type="button" class="elicit-pill" data-value="Quick">Quick</button>
      </div>
    </div>
  </div>
  <div class="elicit-footer">
    <button type="button" class="elicit-skip">Use defaults</button>
    <button type="button" class="elicit-submit">Start</button>
  </div>
</form>
```
