Clutch Arena - go live

1. Upload index.html AND admin.html to Vercel / Netlify (same folder). Open the hosted link, not a chat preview.
   The badge on the home page should say "Live".
2. Admin: log in from the normal Login button with the admin number. The admin panel opens by itself.
   Tabs: Overview, Payments, Rooms, Daily, Bracket.
3. Knockout bracket (admin > Bracket): pick a tournament, press Generate bracket (uses PAID teams only,
   random pairs, byes added automatically), then tap the winner of each match. Players see their opponent,
   Room ID and password under My bookings.

database/ = the base setup SQL only. The live Clutch Arena Supabase project already has it, plus the admin,
daily-tournament and bracket functions added later (those are not in these files). Do NOT run these files
again on that project.

Prize payout flow
- At booking, each player gives a UPI ID (only for paying prize money; other players never see it).
- In a match, each side sees the opponent's captain name and game UID, plus the match Room ID/password.
- After the match, players email the result screenshot to malikkkkkkk20@gmail.com.
- Admin > Bracket: tap the winner of each match. For the final, the panel shows the champion's UPI ID and prize,
  with a "Pay in UPI app" button.
