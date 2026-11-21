# Changelog

## v26.11.21
Completions speaks one visual language: the same marks for the same things everywhere

### Completions

- improved: **Same marks everywhere** for completed, beaten and played
  The year line now reads ★ completed, medal beaten and clock played, like the closed years. The Beaten tag and the group labels carry their mark too.
- improved: **Hardcore** is the same flame tag on beaten rows as on completed cards
  Small enough that the console name still fits on the row.
- fix: **Rarity colours** match the rest of the site
  Ultra rare is under 5% (gold), then Very rare, Rare, Uncommon and Common, as on Analytics and Activity.

### Structure

- fix: **Memory Card** link previews show the new picture after a change
  Discord and WhatsApp kept the first picture they saw for a link. The picture's address now changes whenever the picture does.

## v26.11.20

Eight more Steam games can be marked beaten

### Steam

- improved: **Beaten** marks for Eiyuden Chronicle: Rising and Little Noah: Scion of Paradise
  Each counts as beaten once its final-boss achievement unlocks: This Treasure I've Found and New Journey's Beginning.
- improved: **Beaten** marks for six more story games
  Crimson Desert, Monster Hunter Wilds, Red Dead Redemption 2, Ghost of Tsushima, Assassin's Creed Unity and The Division 2 (all three strongholds).

## v26.11.17
Memory Card's year list is readable by other pages

### Structure

- improved: **Memory Card** publishes every year's title, colour and numbers in `years.json`
  Another page of yours, a home page for example, can draw your years from it.

## v26.11.16
Memory Card's story opens every slide with a line of moving type, plays differently each year, and goes wide on a desktop

### Hub

- new: **Memory Card** story slides open on a cover with a line of moving type
  A full-colour card with one short line about the year, then it opens through a shape onto the slide.
- new: **Memory Card** story plays differently every year, and for every player
  The lines, colours, shapes and the way pieces fly in are drawn from the year and your name, so no two years match and no two players share a story.
- new: **Memory Card** story covers in many more lines and styles
  About 1,700 lines to draw from, and covers that change their typeface, layout, tilt, pattern and the way the number is marked, some with a giant ghost number or a scrolling band.
- improved: **Memory Card** year colour comes from the year's top game
  Each year takes the main colour of its top game's art. Before, six colours took turns by year number.
- new: **Memory Card** story opens wide on a desktop
  Each slide is laid out in two halves to fill the screen. A button in the top bar switches back to the tall cards.
- new: **Memory Card** story cards as wide pictures
  Sharing a slide while the story plays wide sends a 1200 × 630 picture, and the Share sheet's Story section offers the wide ones on a desktop.
- fix: **Memory Card** name in the top bar no longer wraps on narrow phones
- improved: **Memory Card** for the running year opens in July
  A year gets its card once six months of it are done; until then the latest card is last year's.
- fix: **Memory Card** rarest finds in the story no longer squeeze into two columns on a desktop

## v26.11.15
Memory Card, a page to share for each year in games, played back as slides with pictures in five styles, and a list of games to hide from the numbers

### Hub

- new: **Memory Card** a page for each year in games, made to share
  Top five games, the year's days as save blocks, finished games, rarest unlocks, when you play and a title for the year. Share it as a story or wide picture, or as a link that previews that year. Open it from the link under the totals in the header.
- new: **Memory Card** plays the year back as slides, each one a card to share
  Press Play: the year, the top five, finished games, the save blocks with your rhythm, and the rarest finds, one full card each. Tap to step, hold to pause. The share button sends the card on screen as a picture, and the last slide fans out the year's cards over one Share button.
- new: **Memory Card** share pictures in five styles: Card, Cover, Blocks, Shelf and Title
  The Share sheet has three sections, Tall, Wide and Story, each with its pictures as thumbnails to pick from. Shelf shows the year's games as art tiles; Title makes the title you earned the picture.
- improved: **Memory Card** game rows and finished games show their art
  Each top game has its art fading into the row; finished games are tiles with a gold or silver edge. Corners are less round.
- fix: **Memory Card** no more "undefinedm" for top games played before tracking
  A game in the top five with unlocks but no logged play shows its unlock count instead.
- fix: **Memory Card** shows the picture set in Site Config, like the hub

### Analytics

- new: **Hidden games** leave a game out of every number by hand
  Picked in the admin, any platform. Turn it off in the Hide menu like farms.
- improved: **Idle games** keep their unlocks, only their playtime is left out

### Admin

- new: **Hidden Games** page, and a **Timezone** field in Site Config for Memory Card

## v26.11.14
Games from a Steam Family library in your play log, Steam icons that load again, ten more games that can be beaten, and template updates as a pull request

### Steam

- fix: **Icons** for newer games and achievements load again
  Steam stopped serving newer icons from the address the site used; every Steam icon now comes from Steam's current one.
- fix: **Steam Family games** show up in your play log and recently played
  Games you play from someone else's library never appeared, because Steam leaves them out of your own games. Their session times are approximate, to the half hour, because Steam doesn't say when they were last played.
- new: **Beaten markers** for ten more games
  Terraria, Raft, Stardew Valley, Far Cry 3, Monster Hunter Rise, Sekiro, Left 4 Dead 2, Shining Resonance Refrain, TBH: Task Bar Hero and Metro: Last Light (the original release; Redux already had one).

### Structure

- new: **Template updates** arrive as a pull request every Monday
  Merge it to update your site. Your config, series, art picks and avatar are kept. See Getting updates in the README.

## v26.11.11
Your Savepoint hub, ready to fill with your own games.

### Structure

- new: **Savepoint** hub for RetroAchievements, Steam and Xbox
  The hub, a profile page per platform, Activity, Completions, Analytics, Series and this changelog, fed by your own data every hour.
- new: **Admin panel** for series, art, config and data runs
  Runs on your computer with `npm run admin`; never deployed.
- new: **Top bar** starts with the Savepoint wordmark, then your name
- new: **Posters** for your README from your own site: `npm run posters`
