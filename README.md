# Frappe Theme – Minimal Green UI

## Usage
Add the CSS below to:
- `www/custom.css`
- `your_app/public/css/theme.css`
- Website Settings → Custom CSS

Run:
```bash
bench clear-cache
bench restart

Theme CSS
/* =========================
   PRIMARY BUTTONS
   Replace #37715d (primary color)
========================= */
button.btn,
.btn.btn-primary,
.web-footer .btn {
  background-color: #37715d !important;
  border-color: #37715d !important;
  color: #ffffff !important; /* text color */
}

/* =========================
   HOVER / FOCUS
   Replace #30a66d (hover color)
========================= */
button.btn:hover,
.btn.btn-primary:hover,
button.btn:focus,
.btn.btn-primary:focus {
  background-color: #30a66d !important;
  border-color: #30a66d !important;
  color: #ffffff !important;
}

/* =========================
   SECONDARY BUTTONS
   Replace #D9CFE8 (bg)
   Replace #2F2A3A (text)
========================= */
.btn-outline-primary,
.btn-secondary {
  background-color: #D9CFE8 !important;
  border-color: #D9CFE8 !important;
  color: #2F2A3A !important;
}

/* =========================
   LOGIN PAGE BACKGROUND
   Replace #30a66d36 (bg + opacity)
========================= */
.login-content,
.login-wrapper,
.page-card {
  background: #30a66d36 !important;
}

/* =========================
   NAVBAR BACKGROUND
   Replace #30a66d36
========================= */
.navbar,
header,
.page-head {
  background: #30a66d36 !important;
}

/* =========================
   FOOTER BACKGROUND
   Replace #30a66d36
========================= */
.web-footer {
  background: #30a66d36 !important;
}

Color Reference (Replace As Needed)
#37715d   -> Primary buttons
#30a66d   -> Hover / focus state
#D9CFE8   -> Secondary button background
#2F2A3A   -> Secondary button text
#ffffff   -> Button text (recommended no change)
#30a66d36 -> Login, navbar, footer background (hex + alpha)

Notes

36 in #30a66d36 = ~22% opacity

Keep hover color close to primary

Use light backgrounds for login/navbar

Restart bench after changes
