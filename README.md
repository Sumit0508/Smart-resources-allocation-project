# CommuNet — Smart Resource Allocation

> Data-driven volunteer coordination for social impact

Built for the **GDGC Open Innovation Hackathon** — solving the problem of scattered community data and inefficient volunteer deployment for local NGOs and social groups.

---

## The Problem

Local NGOs and social groups collect important community need data through paper surveys, WhatsApp messages, and field reports. This valuable data sits scattered across notebooks and phones — making it impossible to see what is most urgent or where help is needed most. Volunteers get sent to the wrong place, doing the wrong tasks, while real crises go unattended.

---

## The Solution

**CommuNet** is a single platform with three connected modules:

- **Smart Dashboard** — aggregates all field reports into one visual view, showing the most critical community needs at a glance
- **AI-Powered Field Reports** — field workers describe a problem in plain words, and AI automatically detects the category, urgency, severity, and number of people affected
- **Volunteer Matching Engine** — scores every volunteer against each task based on skill match, area proximity, and availability — so the right person goes to the right place

---

## Features

### Dashboard
- Live metrics — total reports, active volunteers, match rate, average response time
- Bar chart showing community needs by category (Healthcare, Food & Water, Education, Shelter, Mental Health)
- Doughnut chart showing urgency distribution (Critical / High / Medium / Low)
- Real-time field report feed that updates instantly when new reports are submitted

### Field Report Submission
- AI Smart Fill — type a plain sentence describing the problem, and Claude AI auto-fills the entire form
- Manual form with ward/area, category, urgency level, people affected, and severity slider
- Submitted reports appear on the dashboard instantly

### Volunteer Hub
- Volunteer profiles with skills, ward area, and weekly availability
- Open task list with urgency indicators
- Smart Match algorithm that scores volunteers out of 100 points:
  - Skill match — 40 points
  - Area proximity — 35 points
  - Availability — 25 points
- Score breakdown bars shown for every volunteer
- Top matched volunteer gets an instant contact card with phone, email, and copy button

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Charts | Chart.js 4.4.1 |
| AI Auto-fill | Anthropic Claude API (claude-sonnet-4-20250514) |
| Hosting | Runs locally via VS Code Live Server |

No backend or database required — fully runs in the browser. Ideal for hackathon demo.

---

## Getting Started

### Prerequisites
- [VS Code](https://code.visualstudio.com/) installed
- [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) installed in VS Code

### Run Locally

1. Clone this repository
```bash
git clone https://github.com/your-sumit0508/communet.git
```

2. Open the folder in VS Code
```bash
cd communet
code .
```

3. Right-click on `index.html` and select **"Open with Live Server"**

4. The app opens in your browser at `http://127.0.0.1:5500`

---

## How to Use

### Submit a Field Report with AI
1. Go to the **Submit Field Report** tab
2. In the green AI Smart Fill box, type something like:
   > *"There are 50 sick children near the school in Ward 3, no medicine available since yesterday"*
3. Click **Auto Fill** — the AI fills all form fields automatically
4. Add your name and click **Submit Field Report**
5. Watch the report appear live on the Dashboard

### Run Smart Volunteer Match
1. Go to the **Volunteer Hub** tab
2. Click any open task from the list
3. Click **Run Smart Match**
4. See all volunteers ranked by score with a breakdown of skill, area, and availability points
5. Contact the top volunteer directly using the contact card

---

## Project Structure

```
communet/
│
└── index.html        # Complete app — all HTML, CSS, and JS in one file
```

---

## Scoring Alignment (Hackathon)

| Criteria | Weight | How we address it |
|---|---|---|
| Technical Merit | 40% | Working AI auto-fill, smart matching algorithm with score breakdown, live dashboard |
| Alignment with Cause | 25% | Directly solves NGO data fragmentation and volunteer misallocation |
| Innovation & Creativity | 25% | AI-powered form filling, transparent scoring logic, real-time updates |
| User Experience | 10% | Clean 3-tab interface, color-coded urgency, instant feedback |

---

## Real World Impact

| Without CommuNet | With CommuNet |
|---|---|
| Data scattered in notebooks and WhatsApp | All reports centralized in one dashboard |
| Coordinators guess what is most urgent | Dashboard surfaces critical needs instantly |
| Volunteers assigned randomly | Matched by skill, area, and availability |
| 2+ days to respond to a crisis | Same-day response with instant contact |

---

## Future Scope

- WhatsApp bot integration for field report submission via chat
- SMS alerts to matched volunteers
- Geographic map view of community needs by ward
- Multi-language support (Tamil, Hindi)
- Real database backend (Firebase / Supabase)
- Mobile app version for field workers

---

## Team

Built with passion for social impact at the GDGC Open Innovation Hackathon.

---

## License

This project is open source and available under the [MIT License](LICENSE).
