# Spacress 1.0 TEST
Native Android Onsen-meguri room-quota puzzle. Android 8+ (min26), target35. Package com.gg007.spacress. Twelve original unique boards on a 4x4 grid.

## Rules
Onsen-meguri on a 4x4 grid divided into four outlined rooms. Draw two separate orthogonal loops, one through each numbered spring. Each loop must contain exactly one circle. The circle number N gives the number of cells that its loop visits in EACH room it enters. A loop may skip a room, but it cannot enter the same room more than once. All four rooms must be visited by at least one loop. Different loops may have different quotas. No crossings, branches or shared cells; unused cells are allowed. Tap gaps between neighboring cells to add/remove links. Twelve original uniquely solved room layouts and distinct solutions; undo/reset, levels and saved palette/optional room letters. Known Onsen-meguri adaptation, with two numbered springs in this edition.

## Download and status
https://mega.co.nz/#!UBcHGQyA!AgBfticLXdNuluRhPSEkeEui2w44LFyHGskKgv4O-gA
APK SHA256 156cec7855ad7404e2166d7e81ccce2ac0e05bfdbb0e5e0b070b579b7aa79b2f; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Portable seed-771110 generator enumerates simple cycles and their 87 vertex-disjoint two-loop unions. It checks 117 connected four-cell room partitions and finds twelve distinct uniquely solved layouts and completions. Every board uses unequal quotas for its two loops. Independent oracle uses disjoint-set components, per-component circle and room counts, and room-internal edge connectivity; production walks each loop cyclically and counts visits and room entries. All 201,326,592 complete edge-state checks plus 120,000 randomized/invalid room-clue cases agree. Bounds, undo/replay/reset and solved lock pass. Actual drawing-adapter edge-midpoint taps solve all twelve and check menu, privacy, levels, next and saved palette/room letters/completion. Seven drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 208 live studio descriptions and the 803-entry web registry. No functional match for per-loop equal room-visit quotas with optional rooms. Springloop compares counts BETWEEN its two loops in each room and requires both loops to visit all rooms. Spacress instead compares each loop with ITSELF across the rooms it chooses: the two loop quotas differ in every generated board, and each loop may skip rooms. Poolcress counts global straight-run lengths, not per-loop room occupancy. Known Onsen-meguri adaptation; original generated layouts, code and visuals, not a global invention. Six sources cover contest rules, constructor posts, implementation history, a player genre index and research context. The contest instruction booklet governs the rules; the Country Road hybrid post is context only, and its extra unused-cell rule is NOT adopted. No source layouts, code or art copied.
Rules https://puzcon.jp/wp-content/plugins/contest-system/documents/20230902/Puzzle%20Getchu!_%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%A9%E3%82%AF%E3%82%B7%E3%83%A7%E3%83%B3%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB.pdf ; independent rules https://ihnnpuzzles.blogspot.com/2024/02/ .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/spacress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.spacress.SpaBoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Spacress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, optional room letters and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 209-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/soazrd1lm999-spacress-source-archive . Repository https://github.com/iLanis-agent/spacress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
