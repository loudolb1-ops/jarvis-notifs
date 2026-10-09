# jarvis-notifs

Réveil de JARVIS : à 12:00, 17:00 et 20:00 (Paris), demande à JARVIS d'envoyer la notif « va poster !! » sur le téléphone de Lou.
Les notifs elles-mêmes (abonnements, envoi Web Push) sont dans JARVIS : `C:\dev\axiom-jarvis\deploy\api\push.js` + `web/sw.js` + bouton « Activer les notifs » de l'onglet Planning.

Secrets : `PUSH_URL` (adresse de `/api/push`), `PUSH_KEY` (la même que la variable Vercel `PUSH_KEY`).
Test immédiat : `gh workflow run va-poster -R loudolb1-ops/jarvis-notifs -f now=true`.
