# Dolomites Guesser

You get a photo, you guess the mountain. Think GeoGuessr, but only for the Dolomites.

## How to play

Open [this](https://gehppappacqi.github.io/DolomitiGuesser/) in a browser. You need internet, since the photos come live from Wikimedia Commons.

- **Multiple choice**: pick the right name out of four.
- **Pinpoint**: drop a pin on the map where you think the peak is. The closer you are, the more points you get.
- Stuck? Hit "Show another angle". It costs you 25 points, but a different photo of the same peak might help.
- 10 rounds per game, and the same peak never shows up twice in one game.

## Curating the photos

Commons search isn't perfect, so some photos are bad (a hut, a blurry shot, the wrong mountain).

- 🚩 **Report** blacklists the photo for good.
- ✅ **Approve** adds it to your hand-picked list for that mountain.
- **Curated mode** only uses approved photos, and only for mountains with at least 2 of them.
- You can hide the Approve/Report buttons if they get in the way.

## Saving your lists

Everything is stored in your browser, so clearing site data wipes it. To keep it safe, press **Export** and you get `blacklist.json`.

If `blacklist.json` sits next to the HTML file and the game is served over http (GitHub Pages, or `python3 -m http.server`), it loads automatically. If you open the file straight from disk, browsers block that, so use **Import** instead.

To share your curation on GitHub Pages: export, replace `blacklist.json` in the repo, commit, done.

## Known quirks

- Peak coordinates for pinpoint mode are from memory, so some may be a couple of km off.
- Entries loaded from `blacklist.json` also get copied into your browser's storage, so deleting one from the file won't remove it until you clear the site data.

Photos from Wikimedia Commons, map imagery from Esri. Have fun, and don't mix up the Tofane with the Cristallo. 🏔
