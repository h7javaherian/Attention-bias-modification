# Attention Bias Modification Task (ABM)
### Dot Probe Paradigm with Emotional Face Stimuli

**Author:** Hoda Haft-Javaherian  
**Built with:** HTML · CSS · JavaScript (no libraries needed)  
**Status:** Complete — ready to use in browser

---

## What is this?

This is a fully functional **Attention Bias Modification (ABM)** research tool built as a single HTML file. It runs entirely in the browser — no installation, no server, no internet connection needed after download.

It implements the **dot probe paradigm**, one of the most widely used tasks in attention and anxiety research, using emotional face stimuli (threat vs. neutral).

---

## What is the dot probe task?

1. A fixation cross (+) appears at the centre of the screen
2. Two faces appear side by side — one **threatening**, one **neutral**
3. The faces disappear, and a **probe** (◆ or ◇) appears where one face was
4. The participant presses **F** (left) or **J** (right) to indicate where the probe appeared
5. Reaction time is recorded

**Key idea:** If someone responds faster when the probe appears at the threat face location, this suggests their attention is automatically drawn toward threat — an **attentional bias**.

---

## Features

| Feature | Details |
|---|---|
| Task modes | Assessment only, ABM training, or both |
| Stimuli | Emotional face pairs (threat vs. neutral) |
| SOA options | 200 ms, 500 ms, 1000 ms |
| Trial counts | 24, 48, or 96 trials |
| Practice phase | 3 practice trials with accuracy feedback |
| Scoring | Automatic Attention Bias Score (ABS) calculation |
| Results dashboard | Summary stats, trial log, RT distribution chart |
| Data export | One-click CSV export with full trial-level data |

---

## How the ABS is calculated

**ABS = RT(incongruent) − RT(congruent)**

- **Congruent trials:** probe appears at the threat face location
- **Incongruent trials:** probe appears at the neutral face location
- **Positive ABS:** attention bias *toward* threat
- **Negative ABS:** attention bias *away from* threat
- **ABS > 15 ms or < -15 ms:** considered clinically meaningful

---

## How to use

**Option 1 — Run directly:**
Download `abm_task.html` and open it in any modern browser (Chrome, Firefox, Safari, Edge). No installation needed.

**Option 2 — Host online:**
Upload to GitHub Pages for a shareable link:
1. Go to repo Settings → Pages
2. Set source to "main branch"
3. Your task will be live at `https://yourusername.github.io/attention-bias-modification-task/abm_task.html`

---

## CSV export format

Each row is one trial. Columns:

| Column | Description |
|---|---|
| participant_id | Entered at session start |
| age | Participant age |
| gender | Participant gender |
| session_type | assess / abm / both |
| soa_ms | Stimulus onset asynchrony in ms |
| date | ISO timestamp of session |
| trial | Trial number |
| threat_left | Whether threat face was on left (true/false) |
| probe_on_threat | Whether probe appeared at threat location |
| probe_position | left or right |
| response | Participant's response (left/right) |
| rt_ms | Reaction time in milliseconds |
| correct | Whether response was correct (true/false) |
| timeout | Whether participant failed to respond in time |

---

## ABM training mode

In ABM training, the probe **always appears at the neutral face location** — never at the threat face. This trains participants to direct attention *away* from threat, which has been studied as a potential intervention for anxiety disorders.

This follows the standard protocol described in:
> MacLeod, C., Rutherford, E., Campbell, L., Ebsworthy, G., & Holker, L. (2002). Selective attention and emotional vulnerability. *Journal of Abnormal Psychology, 111*(1), 107–123.

---

## Clinical relevance

Attention bias toward threat is a well-documented feature of anxiety disorders including:
- Generalized Anxiety Disorder (GAD)
- Social Anxiety Disorder
- PTSD
- Specific phobias

ABM tasks have been studied as both assessment tools and potential therapeutic interventions, making them relevant to clinical research coordination in behavioral health settings.

---

## References

- MacLeod, C., et al. (2002). Selective attention and emotional vulnerability. *Journal of Abnormal Psychology, 111*(1), 107–123.
- Bar-Haim, Y., et al. (2007). Threat-related attentional bias in anxious and nonanxious individuals. *Psychological Bulletin, 133*(1), 1–24.
- Hakamata, Y., et al. (2010). Attention bias modification treatment. *Biological Psychiatry, 68*(11), 982–990.

---

## Contact

**Hoda Haft-Javaherian**  
h7javaherian@gmail.com | Anaheim, CA
