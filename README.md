# CampusConnect

A **full-stack, context-aware dashboard** designed for Mahindra University to dynamically display notices, live match scores, daily themes, and mess menus based on the current context (Daily / Event mode).

---

##  Features

* **Context Switching**

  * Automatically switches between **Daily View** and **Event View (AIRO / AETHER)**

* **Dynamic Notices**

  * Displays real-time announcements from Firebase
  * Filters based on event type (AIRO / AETHER / General)

* **Live Match Dashboard**

  * Displays live sports matches
  * Categorized by sport (Cricket, Football, Basketball)

* **Daily Themes**

  * Event-based themes (e.g., Traditional Wear, Retro Day)
  * Auto-highlights current day

* **Mess Menu System**

  * Displays daily breakfast, lunch, snacks, and dinner

* **Weather Integration**

  * Shows live weather data (temperature, humidity, AQI, etc.)

* **Auto Refresh**

  * Updates data periodically for near real-time experience

---

## Tech Stack

**Frontend**

* HTML, CSS, JavaScript
* Dynamic rendering & context-based UI

**Backend**

* Node.js, Express.js
* REST API architecture

**Database**

* Firebase Firestore

**Deployment**

* Railway (Backend)
* GitHub Pages / Static Hosting (Frontend)
* Netlify

---

## API Endpoints

| Endpoint                | Description                          |
| ----------------------- | ------------------------------------ |
| `/announcements/active` | Fetch active notices                 |
| `/matches/live`         | Get live match scores                |
| `/themes`               | Get daily themes                     |
| `/context/current`      | Determine current mode (Daily/Event) |
| `/weather`              | Fetch weather data                   |

---

## How It Works

1. Frontend fetches data from backend APIs
2. Backend retrieves data from Firebase
3. Context (`AIRO / AETHER / Daily`) determines what is shown
4. UI updates dynamically based on:

   * Selected tab
   * Current context
   * Available data

---

## Context System

| Mode       | Displays                              |
| ---------- | ------------------------------------- |
| **Daily**  | Weather, Mess Menu, Notices, Upcoming |
| **AIRO**   | Sports matches                        |
| **AETHER** | Themes & cultural events              |
| **ALL**    | Everything                            |

---

## Project Structure

```
├── index.html        # Frontend UI
├── server.js         # Backend server (Express)
├── package.json
├── README.md
```

---

## Setup:

### 1. Clone the repo

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

### 2. Install dependencies

```bash
npm install
```

### 3. Add environment variables

Create a `.env` file:

```env
FIREBASE_KEY={your firebase service account JSON}
PORT=7000
```

### 4. Run backend

```bash
node server.js
```

### 5. Run frontend

Open `index.html` in browser or use live server.

---

## Future Improvements


* Admin dashboard for clubs to manage content
* Integration with live sports APIs
* Role-based access for different clubs
* Can add daily food wastage to MENU section
---

## Collaboration Scope

The system can be extended by collaborating with:

* Technical clubs (for automation & scaling)
* Cultural clubs (themes & events)
* Sports clubs (live match data)

---

## Contributors

* Anuj Jandhyala
* Harshith Kottamasu
* Abhinav Simha Dharmana
* Venkat Akshay Grandhi
* Ankit Parupalli
* Aryan Gumidelli
* Gynanesh

