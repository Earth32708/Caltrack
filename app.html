<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CalTrack — Daily log</title>

  <!-- Fonts (same pairing as the landing page) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500&family=Plus+Jakarta+Sans:wght@500;600;700&display=swap" rel="stylesheet">

  <style>
    /* ==========================================================
       1. DESIGN TOKENS — same system as the landing page
       ========================================================== */
    :root {
      --green:       #0E7A5F;
      --green-dark:  #0A5C47;
      --green-soft:  #E3F2EC;
      --coral:       #E8744F;
      --coral-soft:  #FBEAE3;
      --bg:          #FAFAF7;
      --surface:     #FFFFFF;
      --text:        #1F2937;
      --text-muted:  #6B7280;
      --border:      #E5E7EB;
      --error:       #DC2626;
      --warning:     #B45309;

      --radius: 12px;
      --space-1: 8px;
      --space-2: 16px;
      --space-3: 24px;
      --space-4: 32px;

      --font-heading: "Plus Jakarta Sans", sans-serif;
      --font-body: "Inter", sans-serif;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: var(--font-body);
      font-size: 16px;
      line-height: 1.6;
      color: var(--text);
      background: var(--bg);
      min-height: 100vh;
    }

    h1, h2, h3 { font-family: var(--font-heading); line-height: 1.2; }

    .container { max-width: 560px; margin: 0 auto; padding: var(--space-3); }

    a:focus-visible, button:focus-visible, input:focus-visible, select:focus-visible {
      outline: 3px solid var(--coral);
      outline-offset: 2px;
    }

    /* ==========================================================
       2. SHARED PIECES: buttons, inputs, cards
       ========================================================== */
    .btn {
      font-family: var(--font-body);
      font-size: 16px;
      font-weight: 500;
      padding: 12px 24px;
      border-radius: 8px;
      border: none;
      cursor: pointer;
      transition: background 0.15s ease;
    }

    .btn-primary { background: var(--green); color: #fff; }
    .btn-primary:hover { background: var(--green-dark); }

    .btn-secondary {
      background: transparent;
      color: var(--green);
      border: 1.5px solid var(--green);
    }
    .btn-secondary:hover { background: var(--green-soft); }

    .btn-small {
      font-size: 13px;
      padding: 6px 12px;
    }

    input, select {
      font-family: var(--font-body);
      font-size: 16px;
      padding: 11px 14px;
      border: 1px solid var(--border);
      border-radius: 8px;
      background: var(--surface);
      color: var(--text);
      width: 100%;
    }

    label {
      display: block;
      font-size: 14px;
      font-weight: 500;
      margin-bottom: 4px;
    }

    .field { margin-bottom: var(--space-2); }

    .card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: var(--space-3);
      margin-bottom: var(--space-3);
    }

    /* Message shown after errors or successful actions */
    .message {
      font-size: 14px;
      margin-top: var(--space-1);
      min-height: 22px;
    }
    .message.error   { color: var(--error); }
    .message.success { color: var(--green); }

    .hidden { display: none; }

    /* ==========================================================
       3. LOGIN / SIGN UP VIEW
       ========================================================== */
    .auth-wrap { max-width: 420px; margin: 48px auto 0; }

    .auth-logo {
      font-family: var(--font-heading);
      font-weight: 700;
      font-size: 24px;
      text-align: center;
      margin-bottom: var(--space-3);
    }
    .auth-logo span { color: var(--green); }

    .auth-buttons {
      display: flex;
      gap: var(--space-1);
      margin-top: var(--space-2);
    }
    .auth-buttons .btn { flex: 1; }

    /* ==========================================================
       4. APP VIEW (after login)
       ========================================================== */
    .app-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: var(--space-3);
    }

    .app-header .who { font-size: 13px; color: var(--text-muted); }

    /* --- Daily summary --- */
    .summary-numbers {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      margin-bottom: var(--space-1);
    }

    .summary-eaten {
      font-family: var(--font-heading);
      font-weight: 600;
      font-size: 28px;
    }

    .summary-target { font-size: 14px; color: var(--text-muted); }

    .progress-track {
      height: 10px;
      background: var(--green-soft);
      border-radius: 999px;
      overflow: hidden;
    }

    .progress-fill {
      height: 100%;
      width: 0%;
      background: var(--green);
      border-radius: 999px;
      transition: width 0.3s ease;
    }

    /* The bar turns warm orange when over target */
    .progress-fill.over { background: var(--coral); }

    .summary-note {
      font-size: 13px;
      color: var(--text-muted);
      margin-top: var(--space-1);
    }

    /* --- Add food form --- */
    .add-form-row {
      display: grid;
      grid-template-columns: 1fr 110px 130px;
      gap: var(--space-1);
      align-items: end;
    }

    /* --- Entries list --- */
    .entry-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: var(--space-1);
      padding: 10px 0;
      border-top: 1px solid var(--border);
    }
    .entry-row:first-of-type { border-top: none; }

    .entry-meal {
      display: inline-block;
      font-size: 11px;
      font-weight: 500;
      letter-spacing: 0.3px;
      text-transform: uppercase;
      color: var(--green);
      background: var(--green-soft);
      border-radius: 999px;
      padding: 2px 8px;
      margin-right: 6px;
    }

    .entry-kcal { color: var(--text-muted); white-space: nowrap; }

    .delete-btn {
      background: none;
      border: none;
      color: var(--text-muted);
      font-size: 18px;
      cursor: pointer;
      padding: 4px 8px;
      border-radius: 6px;
    }
    .delete-btn:hover { color: var(--error); background: var(--coral-soft); }

    .empty-state {
      text-align: center;
      color: var(--text-muted);
      font-size: 14px;
      padding: var(--space-3) 0;
    }

    /* Mobile: stack the add-food form vertically */
    @media (max-width: 560px) {
      .add-form-row { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>

  <!-- ===================== LOGIN / SIGN UP ===================== -->
  <div id="auth-view" class="auth-wrap hidden">
    <p class="auth-logo">Cal<span>Track</span></p>
    <div class="card">
      <div class="field">
        <label for="email">Email</label>
        <input id="email" type="email" autocomplete="email" placeholder="you@example.com">
      </div>
      <div class="field">
        <label for="password">Password</label>
        <input id="password" type="password" autocomplete="current-password" placeholder="At least 6 characters">
      </div>
      <div class="auth-buttons">
        <button id="login-btn" class="btn btn-primary">Log in</button>
        <button id="signup-btn" class="btn btn-secondary">Sign up</button>
      </div>
      <p id="auth-message" class="message"></p>
    </div>
  </div>

  <!-- ===================== APP (after login) ===================== -->
  <div id="app-view" class="container hidden">

    <div class="app-header">
      <div>
        <h2 id="today-heading">Today</h2>
        <p class="who" id="user-email"></p>
      </div>
      <button id="logout-btn" class="btn btn-secondary btn-small">Log out</button>
    </div>

    <!-- Daily summary -->
    <div class="card">
      <div class="summary-numbers">
        <span class="summary-eaten"><span id="total-kcal">0</span> kcal</span>
        <span class="summary-target">target: <span id="target-kcal"></span> kcal</span>
      </div>
      <div class="progress-track">
        <div id="progress-fill" class="progress-fill"></div>
      </div>
      <p id="summary-note" class="summary-note"></p>
    </div>

    <!-- Add food -->
    <div class="card">
      <div class="add-form-row">
        <div>
          <label for="food-name">Food</label>
          <input id="food-name" type="text" placeholder="e.g. pad krapow">
        </div>
        <div>
          <label for="food-kcal">Calories</label>
          <input id="food-kcal" type="number" min="0" placeholder="540">
        </div>
        <div>
          <label for="food-meal">Meal</label>
          <select id="food-meal">
            <option value="breakfast">Breakfast</option>
            <option value="lunch">Lunch</option>
            <option value="dinner">Dinner</option>
            <option value="snack">Snack</option>
          </select>
        </div>
      </div>
      <div style="margin-top: var(--space-2);">
        <button id="add-btn" class="btn btn-primary">Add to log</button>
      </div>
      <p id="add-message" class="message"></p>
    </div>

    <!-- Today's entries -->
    <div class="card">
      <h3 style="font-size:17px; margin-bottom: var(--space-1);">Logged today</h3>
      <div id="entries-list"></div>
    </div>

  </div>

  <!-- Supabase JavaScript library, loaded from a CDN -->
  <script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>

  <script>
    /* ==========================================================
       1. YOUR SUPABASE PROJECT DETAILS
       Find these in: Supabase dashboard → Project Settings → API
       - Project URL  → goes in SUPABASE_URL
       - "anon public" key → goes in SUPABASE_ANON_KEY
       (The anon key is SAFE to put here. Never put the
        "service_role" key anywhere in frontend code.)
       ========================================================== */
    const SUPABASE_URL = "https://xzmauonotullyizgncas.supabase.co";
    const SUPABASE_ANON_KEY = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Inh6bWF1b25vdHVsbHlpemduY2FzIiwicm9sZSI6ImFub24iLCJpYXQiOjE3ODExNzM2NTksImV4cCI6MjA5Njc0OTY1OX0.kRZp7eDwqpSBBZn9zALu5OvmCnHKtLnYs6GNVFs37Us";

    /* Your daily calorie target. We'll calculate this properly
       from your profile in step 3 — for now, edit it by hand. */
    const DAILY_TARGET = 2000;

    /* ==========================================================
       2. SETUP
       ========================================================== */
    const db = supabase.createClient(SUPABASE_URL, SUPABASE_ANON_KEY);

    // Shortcuts for grabbing elements by their id
    const $ = (id) => document.getElementById(id);

    /* ==========================================================
       3. SHOWING THE RIGHT VIEW (login screen vs the app)
       Supabase tells us whenever the user logs in or out,
       and we show or hide the two views accordingly.
       ========================================================== */
    db.auth.onAuthStateChange((event, session) => {
      if (session) {
        showApp(session.user);
      } else {
        showAuth();
      }
    });

    function showAuth() {
      $("auth-view").classList.remove("hidden");
      $("app-view").classList.add("hidden");
    }

    function showApp(user) {
      $("auth-view").classList.add("hidden");
      $("app-view").classList.remove("hidden");
      $("user-email").textContent = user.email;
      $("target-kcal").textContent = DAILY_TARGET.toLocaleString();
      $("today-heading").textContent = new Date().toLocaleDateString(undefined, {
        weekday: "long", day: "numeric", month: "long"
      });
      loadEntries();
    }

    /* ==========================================================
       4. SIGN UP / LOG IN / LOG OUT
       ========================================================== */
    $("signup-btn").addEventListener("click", async () => {
      const { data, error } = await db.auth.signUp({
        email: $("email").value.trim(),
        password: $("password").value,
      });
      if (error) return showMessage("auth-message", error.message, "error");

      // If email confirmation is turned on in Supabase, there is
      // no session yet and the user must click the link in their inbox.
      if (!data.session) {
        showMessage("auth-message", "Account created! Check your email to confirm, then log in.", "success");
      }
    });

    $("login-btn").addEventListener("click", async () => {
      const { error } = await db.auth.signInWithPassword({
        email: $("email").value.trim(),
        password: $("password").value,
      });
      if (error) showMessage("auth-message", error.message, "error");
    });

    $("logout-btn").addEventListener("click", () => db.auth.signOut());

    /* ==========================================================
       5. LOADING TODAY'S ENTRIES
       Note: we only filter by date here. We do NOT need to filter
       by user — the Row Level Security rules in the database
       already guarantee each person only ever sees their own rows.
       ========================================================== */
    async function loadEntries() {
      const today = new Date().toISOString().slice(0, 10); // "2026-06-12"

      const { data: entries, error } = await db
        .from("log_entries")
        .select("*")
        .eq("eaten_on", today)
        .order("created_at", { ascending: true });

      if (error) {
        showMessage("add-message", "Could not load entries: " + error.message, "error");
        return;
      }
      renderEntries(entries);
    }

    /* ==========================================================
       6. ADDING AN ENTRY
       ========================================================== */
    $("add-btn").addEventListener("click", async () => {
      const name = $("food-name").value.trim();
      const kcal = parseInt($("food-kcal").value, 10);

      // Simple checks before saving
      if (!name) return showMessage("add-message", "Please enter a food name.", "error");
      if (isNaN(kcal) || kcal < 0) return showMessage("add-message", "Please enter the calories.", "error");

      const { data: { user } } = await db.auth.getUser();

      const { error } = await db.from("log_entries").insert({
        user_id: user.id,
        food_name: name,
        calories: kcal,
        meal: $("food-meal").value,
      });

      if (error) return showMessage("add-message", "Could not save: " + error.message, "error");

      // Clear the form and refresh the list
      $("food-name").value = "";
      $("food-kcal").value = "";
      showMessage("add-message", "Added!", "success");
      loadEntries();
    });

    /* ==========================================================
       7. DELETING AN ENTRY
       ========================================================== */
    async function deleteEntry(id) {
      const { error } = await db.from("log_entries").delete().eq("id", id);
      if (error) return showMessage("add-message", "Could not delete: " + error.message, "error");
      loadEntries();
    }

    /* ==========================================================
       8. DRAWING THE LIST AND THE SUMMARY BAR
       ========================================================== */
    function renderEntries(entries) {
      const list = $("entries-list");
      list.innerHTML = "";

      if (entries.length === 0) {
        list.innerHTML = '<p class="empty-state">Nothing logged yet — add your first food above.</p>';
      }

      let total = 0;

      for (const entry of entries) {
        total += entry.calories;

        const row = document.createElement("div");
        row.className = "entry-row";

        const left = document.createElement("span");
        const mealTag = document.createElement("span");
        mealTag.className = "entry-meal";
        mealTag.textContent = entry.meal;
        left.appendChild(mealTag);
        left.appendChild(document.createTextNode(entry.food_name));

        const right = document.createElement("span");
        right.className = "entry-kcal";
        right.textContent = entry.calories.toLocaleString() + " kcal";

        const del = document.createElement("button");
        del.className = "delete-btn";
        del.textContent = "✕";
        del.setAttribute("aria-label", "Delete " + entry.food_name);
        del.addEventListener("click", () => deleteEntry(entry.id));

        row.appendChild(left);
        row.appendChild(right);
        row.appendChild(del);
        list.appendChild(row);
      }

      updateSummary(total);
    }

    function updateSummary(total) {
      $("total-kcal").textContent = total.toLocaleString();

      const percent = Math.min((total / DAILY_TARGET) * 100, 100);
      const fill = $("progress-fill");
      fill.style.width = percent + "%";
      fill.classList.toggle("over", total > DAILY_TARGET);

      const note = $("summary-note");
      if (total > DAILY_TARGET) {
        note.textContent = (total - DAILY_TARGET).toLocaleString() + " kcal over target — tomorrow is a fresh start.";
      } else {
        note.textContent = (DAILY_TARGET - total).toLocaleString() + " kcal remaining today.";
      }
    }

    /* Small helper for showing feedback messages */
    function showMessage(id, text, type) {
      const el = $(id);
      el.textContent = text;
      el.className = "message " + type;
      // Success messages fade away after a moment
      if (type === "success") {
        setTimeout(() => { el.textContent = ""; }, 2500);
      }
    }
  </script>
</body>
</html>
