# TotalCorner API check
Run at 2026-09-11 22:03 UTC

## 1. Token: **OK**
Rate limit 4 of 5 requests left in this minute.
Date requested: 20260912 · page 1 of 43 · 30 matches on this page.

## 2. Coverage on page 1
Leagues on this page: 9

| League | Matches |
| --- | --- |
| Esoccer Battle - 8 mins play | 8 |
| Esoccer H2H GG League - 8 mins play | 6 |
| Esoccer Battle Volta - 6 mins play | 6 |
| Esoccer GT Leagues - 12 mins play | 5 |
| Chile Tercera | 1 |
| Panama Liga Prom | 1 |
| Ecuador LigaPro Serie B | 1 |
| Paraguay Division Profesional | 1 |
| Brazil U20 League | 1 |

## 3. Fields that actually arrive (out of 30 matches)

| Field | Filled | Meaning |
| --- | --- | --- |
| `start` | 30 | kickoff time |
| `l` | 30 | league name |
| `hc` | 9 | home corners |
| `hyc` | 5 | home yellow cards |
| `hrc` | 0 | home red cards |
| `p_odds` | 30 | 1X2 latest price |
| `po_odds` | 30 | 1X2 OPENING price |
| `p_goal` | 30 | goal line |
| `p_corner` | 1 | corner line |
| `p_asian` | 30 | asian handicap |
| `attacks` | 13 | attacks |
| `shot_on` | 26 | shots on target |
| `possess` | 3 | possession |

`po_odds` is the one that matters most: without an opening price there is no Market Moves page.

## 4. One example match (raw)
**Puente Alto v Atletico Oriente** — Chile Tercera — 2026-09-12 00:00:00

```json
{
 "id": "201113875",
 "h": "Puente Alto",
 "h_id": "119458",
 "a": "Atletico Oriente",
 "a_id": "180682",
 "l": "Chile Tercera",
 "l_id": "480",
 "start": "2026-09-12 00:00:00",
 "status": "45",
 "hc": "4",
 "ac": "4",
 "hg": "1",
 "ag": "0",
 "hrc": "0",
 "arc": "0",
 "hyc": "1",
 "ayc": "0",
 "hf_hc": "4",
 "hf_ac": "4",
 "hf_hg": "1",
 "hf_ag": "0",
 "ish": "1",
 "p_odds": [
  "2.875",
  "3.500",
  "2.100"
 ],
 "i_odds": [
  "1.444",
  "4.000",
  "6.500"
 ],
 "po_odds": [
  "2.875",
  "3.500",
  "2.100"
 ],
 "p_asian": [
  "0.0, +0.5"
 ],
 "i_asian": [
  " 0.0"
 ],
 "p_corner": [
  ""
 ],
 "i_corner": [
  ""
 ],
 "p_goal": [
  "3.0"
 ],
 "i_goal": [
  " 2.5"
 ],
 "attacks": [
  "0",
  "1"
 ],
 "attacks_h": [
  "0",
  "0"
 ],
 "dang_attacks": [
  "0",
  "2"
 ],
 "dang_attacks_h": [
  "0",
  "0"
 ],
 "shot_on": [
  "1",
  "0"
 ],
 "shot_on_h": [
  "1",
  "0"
 ],
 "possess": [
  "0",
  "0"
 ],
 "possess_h": [
  "0",
  "0"
 ]
}
```

## 5. Odds history for that match
| List | Entries | First entry |
| --- | --- | --- |
| `odds_list` | 3 | ["45", "1.444", "4.000", "6.500", "2026-09-12 01:03:18", "1", "0"] |
| `goal_list` | 5 | ["45", " 2.5", "1.825", "1.975", "2026-09-12 01:03:18", "1", "0"] |
| `corner_list` | 0 | — |
| `asian_list` | 2 | ["half", " 0.0", "2.000", "1.800", "2026-09-12 00:55:53", "1", "0"] |

Each entry is: match status, line, home price, away price, timestamp, home goal, away goal.

---
API calls used: 2 (limit 30 per minute).