## 🎮 How to Play

### Create an Admin Account
1. Sign up through the app UI.
2. In Supabase, go to Authentication → Users, copy your new user's UID.
3. In the SQL Editor, run:
    ```sql
    UPDATE public.profiles
    SET role = 'admin'
    WHERE id = 'PASTE_YOUR_USER_ID_HERE';
    ```

### Create Participant Accounts
- Sign up for new accounts (default role: participant).

### Start the Hunt!
- Log in as a participant to solve puzzles.
- Log in as admin to watch the leaderboard live.

---

## 🛠️ Tech Stack
- **Frontend:** HTML5, CSS3, JavaScript (Vanilla JS)
- **Backend & Database:** Supabase (PostgreSQL)
- **Authentication:** Supabase Auth
- **Real-Time Engine:** Supabase Realtime

## ⚙️ Setup & Installation

### 1. Backend Setup (Supabase)
1. **Create a Supabase Project:** [supabase.com](https://supabase.com/)
2. **Create Tables:** In the SQL Editor, run SQL scripts to create `profiles`, `checkpoints`, and `progress` tables. *(Paste your SQL here)*
3. **Insert Checkpoints:** Add your checkpoint data. *(Paste your INSERT SQL here)*
4. **Enable Row Level Security (RLS):**
    - Go to Authentication → Policies.
    - Enable RLS for all tables.
    - Add RLS policies. *(Paste your policy SQL here)*

### 2. Frontend Setup
1. **Clone the Repository:**
    ```sh
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    ```
2. **Configure Supabase Credentials:**
    - In your Supabase project, go to Project Settings → API.
    - Copy your Project URL and anon public API Key.
    - Open `index.html`, `dashboard.html`, and `admin.html` and replace the placeholder values:
      ```js
      const SUPABASE_URL = 'YOUR_SUPABASE_URL';
      const SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_KEY';
      ```
3. **Run the Application:**
    - Use a local server (e.g., VS Code Live Server extension).
    - Right-click `index.html` → "Open with Live Server".

# 🗺️ Real-Time Treasure Hunt Platform

>A modern, real-time web app for hosting interactive treasure hunts or checkpoint-based events. Built with vanilla HTML, CSS, and JavaScript, and powered by Supabase for authentication, database, and real-time features.

---

## ✨ Overview
This platform transforms a traditional treasure hunt into a digital, interactive experience:
- **Participants** receive puzzles on their dashboards, travel to physical locations, and scan QR codes to get secret keys. Entering the key unlocks the next challenge and scores points.
- **Admins** get a live dashboard to monitor all participants, scores, and progress in real-time—no refresh needed.

## 🚀 Features

### Participant View
- **Secure Authentication:** Easy sign-up and login.
- **Interactive Dashboard:** See your current puzzle, score, and checkpoint number.
- **Code Validation:** Enter secret codes found at checkpoints.
- **Hints:** Request a hint (with a small point penalty).
- **Skips:** Skip a tough puzzle (with a larger penalty).
- **Real-Time Scoring:** Scores update instantly after each action.
- **Completion Screen:** Get a congratulations message and your final score.

### Admin View
- **Admin Dashboard Screenshot:**  
    <a target="_blank" href=""><img src="https://imghost.online/ib/tHcxWZBe71IxtuX_1754169005.png" alt="Admin Dashboard Screenshot"/></a>
- **Role-Based Access:** Only admins can access the admin dashboard.
- **Live Leaderboard:** See all participants, their scores, and current checkpoint in real-time.
- **Real-Time Monitoring:** Powered by Supabase subscriptions for instant updates.
## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3, JavaScript (Vanilla JS)
- **Backend & Database:** Supabase (PostgreSQL)
- **Authentication:** Supabase Auth
- **Real-Time Engine:** Supabase Realtime

## ⚙️ Setup & Installation

### 1. Backend Setup (Supabase)
1. **Create a Supabase Project:** Sign up at [supabase.com](https://supabase.com/) and create a new project.
3. **Insert Checkpoints:** Add your checkpoint data using SQL INSERT statements. *(Paste your INSERT SQL here)*the Supabase dashboard, open the SQL Editor and run scripts to create the `profiles`, `checkpoints`, and `progress` tables. *(Paste your SQL here)*
4. **Enable Row Level Security (RLS):**
    - Go to Authentication → Policies.To get this project running on your own, follow these steps.
    - Enable RLS for all tables.
    - Add RLS policies as needed. *(Paste your policy SQL here)*
You need a free Supabase account.
### 2. Frontend Setup
1. **Clone the Repository:**
    ```sh<summary><strong>Click here for step-by-step Supabase configuration</strong></summary>
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-nameCreate a New Project: Go to Supabase and create a new project.
    ```
2. **Configure Supabase Credentials:**Run SQL Scripts: In the Supabase dashboard, go to the SQL Editor and run the following scripts to create the tables and add the initial data.
    - In your Supabase project, go to Project Settings → API.
    - Copy your Project URL and anon public API Key.Create Tables Script:
    - Open `index.html`, `dashboard.html`, and `admin.html` and replace the placeholder values:
      ```js
      const SUPABASE_URL = 'YOUR_SUPABASE_URL';-- (Paste the full SQL from the previous instructions here)
      const SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_KEY';
      ```Insert Checkpoints Script:
3. **Run the Application:**
    - Use a local server (e.g., VS Code Live Server extension).
    - Right-click `index.html` → "Open with Live Server".-- (Paste the INSERT SQL from the previous instructions here)

