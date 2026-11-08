# Dropcress 1.0 TEST
Native Android SameGame group-clearing puzzle. Android 8+ (min26), target35. Package com.gg007.dropcress. Twelve original full-clear starts on a compact 4x3 board.

## Rules
SameGame training puzzle on a 4-column by 3-row board with three colors, always labeled A, B, C. Tap any tile in a side-connected group of two or more matching symbols to remove the WHOLE group. Diagonal contact does not join tiles. Surviving tiles first fall straight DOWN within each column, preserving vertical order. Then all empty columns close to the LEFT, preserving column order. Newly touching groups remain until you tap them; no automatic chains, new tiles, recoloring or manual swaps. Goal: remove EVERY tile, then CHECK. A nonempty board of isolated singles is a dead end, not a win; unlimited UNDO or RESET remains available. Twelve original solvable starts, shortest clears of 4 or 5 removals. Multiple successful sequences can exist. This smaller training adaptation has one-tap removal, no selection preview and no point scoring; it focuses on full clearance rather than maximizing a score. NEXT, levels, saved palette and optional a-l cell guides. A/B/C symbols stay visible even when guides are off.

## Download and status
https://mega.co.nz/#!Bc103AyA!5wKtDOL-YH9w3SfGYEoMsdC7YkiAy0LOJesVnQjLMf4
APK SHA256 2e8c1076c77f669b7d07c88a56c73628b5a4aa07b60b724e0b34b45a3b2c6d56; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent union-find grouping and survivor-list compaction agree with production flood-growth bitmask grouping and bottom-up gravity/column packing in 200,004 comparisons. Coverage: all 4,096 complete two-color boards, 10,000 seeded mixed/empty boards, and all 190 states reachable across the twelve original starts. Each reachable tile choice, including invalid index and singleton cases, checked. Independent breadth-first searches prove shortest full clears 4,5,4,4,4,4,4,4,5,5,4,4. Color/column order and at-least-two removal invariants pass, along with invalid state, early check, undo, solved lock, reset and replay. Archived portable generator reproduces levels and archived Java oracle reruns byte-equal. Actual drawing-adapter group taps, gravity, solve/undo/replay, menu, levels, privacy and saved palette/cell guides pass. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 176 prior studio mechanics and all 803 web registry records for functional overlap. Fifteen was rejected because web Fifteen already has the same adjacent-blank algorithm. Dropcress instead removes complete equal-symbol components and applies downward gravity plus leftward empty-column compression. Flood It recolors an expanding corner territory without removing tiles; 2048 slides and merges values; TileTug shifts rows and chains matches in a tug contest. None has this group-removal and two-stage compaction planning problem in the reviewed catalog. Known SameGame/Clickomania adaptation, not a global invention claim. Original generated starts, implementation and visuals; no source boards, code or art copied. Recovered repository corpus remains partial.
Rules https://erikdemaine.org/clickomania/ ; independent rules https://www.janko.at/Spiele/SameGame/Regeln-en.htm .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/dropcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.dropcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Dropcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, cell guides and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 177-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/jzqibdwtxdfm-dropcress-source-archive . Repository https://github.com/iLanis-agent/dropcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
