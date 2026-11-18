# Klyx Privacy Policy

**Last updated: November 17, 2026**

Klyx is a Discord bot with a web dashboard. This policy explains what data Klyx uses, why, and how you can have it deleted. Klyx is operated by D3f4ultscript.

Contact: open an issue at https://github.com/D3f4ultscript/Klyx-Discord-Bot/issues (or ask in the Klyx support server, if one is linked on the website).

## 1. What Klyx stores

Klyx only stores what it needs to work.

| Data | Why | Details |
|---|---|---|
| Server settings | To run the features an admin turned on | Channel IDs, role IDs, message templates, filter lists, language |
| Warnings | Moderation | User ID, moderator ID, reason, time, server ID |
| Levels | XP and level system, rank cards and the leaderboard | User ID, XP, level, server ID, display name and avatar link (for the leaderboard). XP can come from messages, voice time and reactions, depending on the server settings. Voice time and reactions are only counted, not stored |
| Giveaways | Run giveaways | Prize, channel and message IDs, host ID, requirements set by the host, the IDs of members who entered, winner IDs |
| Invite tracker | Show who invited whom, if the admin turned it on | Server ID, the joining user's ID, the inviter's ID, invite code, join time, whether the member left, whether the account counted as new. Bonus invites given by admins |
| Birthdays | Congratulate members | Server ID, user ID, day and month (no year). Saved only when the member uses `/birthday set`, deleted with `/birthday remove` |
| Reputation | Points members give each other | Server ID, user ID, points. Who gave a point to whom and when, kept for 8 days for the cooldown |
| Highlights | DM a member when a word they follow is said | Server ID, user ID, the words the member added |
| Counting | The counting game | Server ID, current number, best number, the ID of the last member who counted |
| Temporary voice channels | Delete them when they are empty | Channel ID, server ID, owner ID, creation time |
| Tickets | Support tickets | Server ID, channel ID, user ID, ticket number and type, who claimed it, who closed it, who answered first and when, priority, status, open and close time, close reason, the star rating and the optional rating comment if the member gave one |
| Suggestions | Collect ideas and let members vote | Server ID, user ID of the author, the suggestion text, time, status and decision reason, and each member's vote (user ID, up or down) |
| Honeypot | Catch scam bots in a trap channel, if the admin turned it on | Server ID, user ID, channel ID, time, action taken, and the first 500 characters of the message. Deleted after 180 days |
| Reminders | `/remind` | User ID, channel ID, reminder text, time |
| Reaction roles | Give roles for reactions | Server ID, message ID, emoji, role ID |
| Moderation cases | Case numbers and moderation history | Server ID, user ID, moderator ID, action, reason, time |
| Security events | Show admins what the security features did | Server ID, user ID, type of event (for example raid, scam link, quarantine), a short description, time. Klyx keeps the last 300 per server |
| Quarantine | Give members their roles back after a quarantine | Server ID, user ID, the IDs of the removed roles, reason, time |
| Verification | Kick members who do not verify in time, if the admin turned that on | Server ID, user ID, join time. Deleted once the member verifies or leaves |
| Saved roles | Give members their roles back when they rejoin, if the admin turned that on | Server ID, user ID, role IDs, time. Deleted after rejoining or after 30 days |
| AutoMod violations | Punish repeated rule breaking harder, if the admin set up escalation | Server ID, user ID, time of each violation. Deleted after 7 days |
| Temporary roles | Remove a role again when its time is up | Server ID, user ID, role ID, end time |
| Server backups | Rebuild roles and channels after an attack | Names, permissions and settings of roles, categories and channels. No members and no messages. Klyx keeps the last 5 per server |

Klyx does **not** store the content of chat messages in its database. Messages are read in memory to run AutoMod, the scam link filter and the level system and are discarded afterwards.

If a server admin turns on the public leaderboard, the top 100 members of that server are shown on the Klyx website with display name, avatar, level and XP. Anyone with the link can see this page. Welcome picture cards are made on the fly from the member's avatar and name and are not stored.

To detect scam links, Klyx downloads public lists of known scam domains every few hours. Nothing about your server or your members is sent anywhere for this check. Captcha and math answers for verification only live in memory for a few minutes. To protect servers from attacks, Klyx reads the server's audit log (who banned, kicked, deleted or created what) while it happens and only keeps it in memory for a few minutes.

## 2. Content that Klyx posts to your server

If a server admin turns on the server log or the moderation log, Klyx posts embeds to the log channel the admin chose. These can contain the text of deleted or edited messages, AutoMod hits and moderation actions. This content stays inside that Discord server and is controlled by the server's admins. When a ticket is closed, a text transcript is posted to the log channel chosen by the admin and is not kept by Klyx. When a member reports a message, Klyx posts its text, author and a link to it in the report channel chosen by the admin. Answers to ticket questions and forms are posted in the channel chosen by the admin and are not kept by Klyx. If the admin turned it on, the member also gets the ticket transcript by DM.

Feeds: if an admin adds an RSS or YouTube feed, Klyx loads that public address every 15 minutes and stores only an ID of each post it has seen, for 60 days.

## 3. Dashboard login

When you log in to the dashboard with Discord (OAuth2, scopes `identify` and `guilds`), Klyx receives your Discord user ID, name, avatar and the list of servers you are in. Klyx uses this list only to show the servers where you have the Manage Server permission. If a server set up manager roles, Klyx also checks your roles on that server through Discord's API to decide whether you may open its dashboard. The access token is used once during login and is not stored. The server list is kept in server memory for 15 minutes and is not written to the database.

The dashboard uses one technical session cookie (signed, no tracking) that keeps you logged in and protects forms. Klyx uses no advertising or analytics cookies.

## 4. Sharing

Klyx does not sell data and does not share it with third parties. Data is processed through Discord's API. Donations are made through PayPal or cryptocurrency wallets. Klyx does not process payments and does not store payer data.

## 5. How long data is kept

Data is kept while Klyx is on the server or until it is deleted. Warnings, levels and reminders can be removed by server moderators with the bot commands, for example `/delwarn`, `/clearwarnings`, `/xp reset`, or by removing Klyx from the server and requesting deletion.

## 6. Your rights and deletion

You can ask for access to your data or for its deletion at any time. Server admins can ask for all data of their server to be deleted. Send the request through the contact option above and include your Discord user ID or server ID. Requests are handled within 30 days.

## 7. Children

Klyx follows Discord's minimum age. You must be at least 13 years old (or older if your country requires it) to use Discord and therefore Klyx.

## 8. Security

Data is stored on the server that runs Klyx. Access is limited to the operator. No system is perfectly secure, so Klyx stores as little as possible.

## 9. Changes

This policy can change when Klyx gets new features. The date at the top shows the latest version.

---

# Klyx Datenschutzerklärung

**Stand: 17. November 2026**

Klyx ist ein Discord-Bot mit Web-Dashboard. Diese Erklärung sagt, welche Daten Klyx nutzt, wofür, und wie du sie löschen lassen kannst. Betreiber von Klyx ist D3f4ultscript.

Kontakt: eröffne ein Issue unter https://github.com/D3f4ultscript/Klyx-Discord-Bot/issues (oder frag im Klyx-Support-Server, falls einer auf der Website verlinkt ist).

## 1. Was Klyx speichert

Klyx speichert nur, was es zum Funktionieren braucht.

| Daten | Wofür | Einzelheiten |
|---|---|---|
| Server-Einstellungen | Funktionen, die ein Admin eingeschaltet hat | Kanal-IDs, Rollen-IDs, Nachrichtenvorlagen, Filterlisten, Sprache |
| Verwarnungen | Moderation | Nutzer-ID, Moderator-ID, Grund, Zeit, Server-ID |
| Levels | XP- und Level-System, Rang-Karten und Bestenliste | Nutzer-ID, XP, Level, Server-ID, Anzeigename und Avatar-Link (für die Bestenliste). XP kann je nach Server-Einstellung aus Nachrichten, Voice-Zeit und Reaktionen kommen. Voice-Zeit und Reaktionen werden nur gezählt, nicht gespeichert |
| Gewinnspiele | Gewinnspiele durchführen | Preis, Kanal- und Nachrichten-IDs, Veranstalter-ID, vom Veranstalter gesetzte Anforderungen, IDs der Teilnehmer, Gewinner-IDs |
| Einladungs-Tracker | Zeigen, wer wen eingeladen hat, wenn der Admin das eingeschaltet hat | Server-ID, ID des beitretenden Nutzers, ID des Einladenden, Einladungscode, Beitrittszeit, ob das Mitglied gegangen ist, ob der Account als neu zählte. Bonus-Einladungen, die Admins vergeben |
| Geburtstage | Mitgliedern gratulieren | Server-ID, Nutzer-ID, Tag und Monat (kein Jahr). Nur gespeichert, wenn das Mitglied `/birthday set` nutzt, gelöscht mit `/birthday remove` |
| Reputation | Punkte, die Mitglieder sich gegenseitig geben | Server-ID, Nutzer-ID, Punkte. Wer wem wann einen Punkt gegeben hat, 8 Tage lang für den Cooldown |
| Highlights | Einem Mitglied eine DM senden, wenn ein Wort fällt, dem es folgt | Server-ID, Nutzer-ID, die Wörter, die das Mitglied hinzugefügt hat |
| Zählen | Das Zählspiel | Server-ID, aktuelle Zahl, Rekord, ID des Mitglieds, das zuletzt gezählt hat |
| Temporäre Sprachkanäle | Sie löschen, wenn sie leer sind | Kanal-ID, Server-ID, Besitzer-ID, Erstellzeit |
| Tickets | Support-Tickets | Server-ID, Kanal-ID, Nutzer-ID, Ticketnummer und Art, wer es übernommen hat, wer es geschlossen hat, wer zuerst geantwortet hat und wann, Priorität, Status, Öffnungs- und Schließzeit, Schließgrund, die Sterne-Bewertung und der freiwillige Bewertungs-Kommentar, falls das Mitglied sie abgegeben hat |
| Vorschläge | Ideen sammeln und abstimmen lassen | Server-ID, Nutzer-ID des Autors, Text des Vorschlags, Zeit, Status und Grund der Entscheidung sowie die Stimme jedes Mitglieds (Nutzer-ID, dafür oder dagegen) |
| Honeypot | Scam-Bots in einem Fallen-Kanal erwischen, wenn der Admin das eingeschaltet hat | Server-ID, Nutzer-ID, Kanal-ID, Zeit, ergriffene Aktion und die ersten 500 Zeichen der Nachricht. Nach 180 Tagen gelöscht |
| Erinnerungen | `/remind` | Nutzer-ID, Kanal-ID, Erinnerungstext, Zeit |
| Reaktionsrollen | Rollen für Reaktionen vergeben | Server-ID, Nachrichten-ID, Emoji, Rollen-ID |
| Moderations-Fälle | Fallnummern und Moderations-Akte | Server-ID, Nutzer-ID, Moderator-ID, Aktion, Grund, Zeit |
| Sicherheits-Ereignisse | Admins zeigen, was die Sicherheitsfunktionen getan haben | Server-ID, Nutzer-ID, Art des Ereignisses (zum Beispiel Raid, Betrugs-Link, Quarantäne), kurze Beschreibung, Zeit. Klyx behält die letzten 300 pro Server |
| Quarantäne | Mitgliedern nach einer Quarantäne ihre Rollen zurückgeben | Server-ID, Nutzer-ID, IDs der entfernten Rollen, Grund, Zeit |
| Verifizierung | Mitglieder kicken, die sich nicht rechtzeitig verifizieren, wenn der Admin das eingeschaltet hat | Server-ID, Nutzer-ID, Beitrittszeit. Wird gelöscht, sobald das Mitglied sich verifiziert oder geht |
| Gespeicherte Rollen | Mitgliedern ihre Rollen zurückgeben, wenn sie wieder beitreten, falls der Admin das eingeschaltet hat | Server-ID, Nutzer-ID, Rollen-IDs, Zeit. Gelöscht nach dem Wiederbeitritt oder nach 30 Tagen |
| AutoMod-Verstöße | Wiederholte Verstöße härter bestrafen, falls der Admin eine Steigerung eingerichtet hat | Server-ID, Nutzer-ID, Zeitpunkt jedes Verstoßes. Gelöscht nach 7 Tagen |
| Rollen auf Zeit | Eine Rolle wieder entfernen, wenn ihre Zeit abgelaufen ist | Server-ID, Nutzer-ID, Rollen-ID, Ablaufzeit |
| Server-Backups | Rollen und Kanäle nach einem Angriff wiederherstellen | Namen, Rechte und Einstellungen von Rollen, Kategorien und Kanälen. Keine Mitglieder und keine Nachrichten. Klyx behält die letzten 5 pro Server |

Klyx speichert den Inhalt von Chat-Nachrichten **nicht** in der Datenbank. Nachrichten werden im Arbeitsspeicher für AutoMod, den Betrugs-Link-Filter und das Level-System gelesen und danach verworfen.

Schaltet ein Server-Admin die öffentliche Bestenliste ein, werden die Top 100 Mitglieder dieses Servers mit Anzeigename, Avatar, Level und XP auf der Klyx-Website gezeigt. Jeder mit dem Link kann diese Seite sehen. Willkommens-Bildkarten werden beim Beitritt aus Avatar und Name erzeugt und nicht gespeichert.

Um Betrugs-Links zu erkennen, lädt Klyx alle paar Stunden öffentliche Listen bekannter Betrugs-Domains herunter. Dabei wird nichts über deinen Server oder deine Mitglieder irgendwohin gesendet. Captcha- und Rechen-Antworten zur Verifizierung liegen nur ein paar Minuten im Arbeitsspeicher. Um Server vor Angriffen zu schützen, liest Klyx das Audit-Log des Servers (wer was gebannt, gekickt, gelöscht oder erstellt hat) in dem Moment, in dem es passiert, und behält es nur ein paar Minuten im Arbeitsspeicher.

## 2. Inhalte, die Klyx auf deinem Server postet

Schaltet ein Server-Admin das Server-Log oder das Moderations-Protokoll ein, postet Klyx Embeds in den vom Admin gewählten Log-Kanal. Diese können den Text gelöschter oder bearbeiteter Nachrichten, AutoMod-Treffer und Moderationsaktionen enthalten. Diese Inhalte bleiben auf diesem Discord-Server und werden von dessen Admins kontrolliert. Beim Schließen eines Tickets wird ein Textprotokoll in den vom Admin gewählten Log-Kanal gepostet und von Klyx nicht aufbewahrt. Meldet ein Mitglied eine Nachricht, postet Klyx deren Text, den Autor und einen Link dazu in den vom Admin gewählten Meldekanal. Antworten auf Ticket-Fragen und Formulare werden in den vom Admin gewählten Kanal gepostet und von Klyx nicht aufbewahrt. Hat der Admin das eingeschaltet, bekommt das Mitglied das Ticket-Protokoll zusätzlich per DM.

Feeds: Fügt ein Admin einen RSS- oder YouTube-Feed hinzu, lädt Klyx diese öffentliche Adresse alle 15 Minuten und speichert nur eine ID jedes gesehenen Beitrags, für 60 Tage.

## 3. Dashboard-Login

Wenn du dich mit Discord im Dashboard anmeldest (OAuth2, Bereiche `identify` und `guilds`), erhält Klyx deine Discord-Nutzer-ID, deinen Namen, dein Profilbild und die Liste deiner Server. Klyx nutzt diese Liste nur, um die Server zu zeigen, auf denen du das Recht Server verwalten hast. Hat ein Server Manager-Rollen eingerichtet, prüft Klyx zusätzlich über die Discord-API deine Rollen auf diesem Server, um zu entscheiden, ob du sein Dashboard öffnen darfst. Das Zugriffstoken wird einmal beim Login benutzt und nicht gespeichert. Die Serverliste liegt 15 Minuten im Arbeitsspeicher des Servers und wird nicht in die Datenbank geschrieben.

Das Dashboard nutzt ein technisches Sitzungs-Cookie (signiert, ohne Tracking), das dich angemeldet hält und Formulare schützt. Klyx nutzt keine Werbe- oder Analyse-Cookies.

## 4. Weitergabe

Klyx verkauft keine Daten und gibt sie nicht an Dritte weiter. Die Daten werden über die Discord-API verarbeitet. Spenden laufen über PayPal oder Krypto-Wallets. Klyx wickelt keine Zahlungen ab und speichert keine Daten von Spendern.

## 5. Wie lange Daten gespeichert werden

Daten bleiben gespeichert, solange Klyx auf dem Server ist oder bis sie gelöscht werden. Verwarnungen, Levels und Erinnerungen können Server-Moderatoren mit Bot-Befehlen entfernen, zum Beispiel `/delwarn`, `/clearwarnings`, `/xp reset`, oder indem Klyx vom Server entfernt und die Löschung beantragt wird.

## 6. Deine Rechte und Löschung

Du kannst jederzeit Auskunft über deine Daten oder deren Löschung verlangen. Server-Admins können die Löschung aller Daten ihres Servers verlangen. Schicke die Anfrage über den Kontakt oben und gib deine Discord-Nutzer-ID oder Server-ID an. Anfragen werden innerhalb von 30 Tagen bearbeitet.

## 7. Kinder

Klyx richtet sich nach dem Mindestalter von Discord. Du musst mindestens 13 Jahre alt sein (oder älter, wenn dein Land es verlangt), um Discord und damit Klyx zu nutzen.

## 8. Sicherheit

Die Daten liegen auf dem Server, auf dem Klyx läuft. Zugriff hat nur der Betreiber. Kein System ist perfekt sicher, deshalb speichert Klyx so wenig wie möglich.

## 9. Änderungen

Diese Erklärung kann sich ändern, wenn Klyx neue Funktionen bekommt. Das Datum oben zeigt die neueste Fassung.
