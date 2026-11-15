# Changelog

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
