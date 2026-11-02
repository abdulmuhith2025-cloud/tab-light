# Tab Light — Render beta

This folder packages the supplied Tab Light HTML prototype with its small Express API. The API powers only the Zayed beta endpoint; it does not add accounts, a database, protected admin access, journal-index verification, or persistent user data.

## Deploy

1. Push this folder to a GitHub repository. When creating the Render Web Service, set **Root Directory** to `render-deploy` if this folder is inside a larger repository.
2. Select Node, Free instance, build command `npm install`, and start command `npm start`.
3. Render uses `/health` as the health check. The frontend and API are served from the same `onrender.com` host.
4. To turn on Zayed's model call, create an API key in Google AI Studio and add it in the Render service's Environment settings as `GEMINI_API_KEY`. Add `GEMINI_MODEL` using a model currently available to that key. Never put the key in GitHub, HTML, or this chat.
5. Keep `ALLOW_UNREVIEWED_BETA=false` until an editor verifies the source collection. With the current collection, Zayed should refuse to produce a tafsir answer until eligible material is reviewed and published.

## Beta boundaries

- The included source collection contains unreviewed Quran entries and no verified tafsir entries. Do not present its generated output as scholarly-validated tafsir.
- Registration and the admin area are demonstrations only. There is no authentication or database.
- Prayer time is calculated in the browser from user-entered coordinates and is explicitly not an official timetable.
- Render's free web services can sleep when idle; the first request after sleep may be delayed. This deployment is for a test, not a production guarantee.
