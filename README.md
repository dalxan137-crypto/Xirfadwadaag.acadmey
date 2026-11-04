# Xirfad Wadaag Academy

Two standalone pages (prototype, data kept in the browser only):

- `index.html`: public website (courses, enrolment, student dashboard, certificate verification).
- `admin.html`: admin dashboard, opened with the admin PIN (demo PIN: 2026, change it in Settings).

## Going live
The prototype stores data in each browser's localStorage, so the two pages do not share data.
For production you need:
- A database (for example Supabase) shared by both pages.
- Server-side login and a real admin account; move the PIN check to the server.
- Payment confirmation from the mobile money provider (webhook or merchant API), not manual entry.
- Private video hosting with signed URLs (for example Bunny Stream or Cloudflare Stream).
