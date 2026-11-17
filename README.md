City Clean-Up — Open Source & SDG Classroom Quiz Game

An interactive classroom quiz game that combines learning, teamwork, environmental awareness, and a playful city-restoration experience. Students answer quiz questions, earn points, and clean up a virtual city together.

> Project update: The Meow Coins economy, customization shop, and “Save Mr. Meow!” winter mini-game below describe the new feature scope supplied for this project. They should be marked as implemented only after the corresponding changes are added to the application.

Current Game

Main Features

 ● Interactive city map: Select one of 10 trash hotspots to open a quiz question.
 ● Three team modes: Play as a whole class, or split the class into 2 or 3 teams.
 ● 30 quiz questions: Questions are divided into three waves of 10, with an option to play 10 random questions.
 ● Question editor: Add, edit, and delete questions, or import multiple questions at once.
 ● Bilingual interface: Switch between Russian and English.
 ● Team scoring: Correct answers award 100 points and clean the selected area.
 ● City restoration: Track the city’s cleanliness as quiz areas are cleared.
 ● Learning feedback: Incorrect answers show a hint; correct answers show an explanation or fact.
 ● Mr. Meow mascot: An animated cat assistant reacts during gameplay.
 ● Sound and animations: Includes sound effects, animated city elements, and visual feedback.
 ● Responsive layout: Designed for classroom displays and mobile screens.

New Feature Scope

1. Meow Coins Economy and Shop

The planned in-game economy rewards learning progress with Meow Coins.

Earning coins

|Action                         |Reward          |
|-——————————|—————:|
|Correct answer                 |+10 coins       |
|Correct answer within 5 seconds|+5 bonus coins  |
|3 correct answers in a row     |+10 streak bonus|
|5 correct answers in a row     |+20 streak bonus|
|10 correct answers in a row    |+50 streak bonus|
|Incorrect answer               |0 coins         |

The coin balance should be visible in the main interface, animate when coins are earned, and persist between sessions. The system should prevent negative balances and duplicate rewards for the same question.

Shop categories

Mr. Meow’s Wardrobe

|Cosmetic item      |Price|
|-——————|-—:|
|Sunglasses 😎       |30   |
|Graduation cap 🎓   |40   |
|Crown 👑            |100  |
|Wizard hat 🪄       |80   |
|Superhero costume 🦸|150  |
|Pirate outfit 🏴‍☠️    |120  |
|Hoodie 👕           |90   |
|Golden chain ⛓️     |70   |

Purchased outfits should be added to the inventory. Players should be able to equip or unequip owned items, and Mr. Meow’s appearance should update immediately.

City Decorations

|Decoration             |Price|
|————————|-—:|
|Flowers 🌸              |20   |
|Small tree 🌳           |40   |
|Bench 🪑                |50   |
|Street lamp 💡          |60   |
|Fountain ⛲️             |120  |
|Colorful playground 🛝  |150  |
|Flower garden 🌷        |100  |
|Solar panels ☀️         |180  |
|Recycling station ♻️    |80   |
|Eco-friendly building 🏡|250  |

Purchased decorations should be added to the player’s inventory and displayed in the city. If supported by the city architecture, players should also be able to reposition placed decorations.

Shop experience

The planned shop includes category tabs, a live coin balance, item prices, purchase and ownership statuses, a Mr. Meow outfit preview, and decoration previews. Mr. Meow should react to purchases and display funny messages when the player cannot afford an item.

2. City Customization and Progression

The shop is intended to work together with the existing city-restoration mechanic:

 ● Trees and flowers make the environment greener and more colorful.
 ● Benches and street lamps make the city more welcoming.
 ● Recycling stations reinforce the sustainability theme.
 ● Solar panels represent clean energy.
 ● Eco-friendly buildings help create a greener city.

The goal is to let players see the difference between the original polluted city and their customized, restored environment.

3. “Save Mr. Meow!” Winter Mini-Game

An optional arcade-style mini-game inside the existing application. It is an additional activity, not a replacement for the main quiz.

Story: Mr. Meow is freezing in a snowy environment. The player must collect resources to help him get warm.

Gameplay

 ● 45-second countdown.
 ● Move left and right using keyboard arrows or mobile touch controls.
 ● Collect useful resources while avoiding obstacles.

Required resources

|Resource  |Required amount|
|-———|—————:|
|Wood 🪵    |5              |
|Wool 🧶    |3              |
|Firewood 🔥|3              |
|Fish 🐟    |2              |

Obstacles: Ice blocks 🧊, trash 🗑️, and snowballs ❄️.

A resource inventory and warmth meter show the player’s progress. When the player succeeds, the game shows Mr. Meow becoming warm and happy, with a shelter, blanket, campfire, and fish.

Completion reward

 ● +100 Meow Coins.
 ● Exclusive winter hat for Mr. Meow.
 ● Achievement: Cat Savior 🐾.

The reward should be granted only once, even if the mini-game is replayed. Failure should allow the player to retry or return to the main game without losing existing coins or progress.

How to Run

The current project is a standalone HTML application. No installation or build process is required.

 1. Download or clone this repository.
 2. Open city_clean_up_classroom_quiz_game.html in a modern web browser.
 3. Start the game and choose a question wave and team mode.
 4. Click a glowing hotspot on the city map to answer a question.

> Note: The current HTML page loads Tailwind CSS and Google Fonts from external CDNs. An internet connection is required for those external resources to load correctly. The current game does not require a backend server.

How to Play the Main Quiz

 1. Choose a question set:
 ● Wave 1: Questions 1–10
 ● Wave 2: Questions 11–20
 ● Wave 3: Questions 21–30
 ● Random 10: A random set of 10 questions
 2. Select a team mode: Whole Class, 2 Teams, or 3 Teams.
 3. Select an uncleared hotspot on the city map.
 4. Read the question and choose one of the four answers.
 5. A correct answer awards 100 points and clears that city area.
 6. An incorrect answer displays a hint. In team modes, the turn passes to the next team.
 7. Continue until all active areas are clean and the victory screen appears.

Keyboard Shortcuts

|Key               |Action                                   |
|——————|——————————————|
|`1`–`9`           |Open hotspots 1–9                        |
|`0`               |Open hotspot 10                          |
|`A`, B, C, `D`|Select an answer                         |
|`1`, 2, 3, `4`|Select an answer                         |
|`Enter` or `Space`|Continue after answering                 |
|`Esc`             |Close the current modal                  |
|Arrow keys        |Planned controls for the winter mini-game|

Russian keyboard equivalents for answer selection are also supported: Ф, И, С, В.

Customizing Quiz Questions

Use the Questions button in the game to open the built-in question editor.

You can:

 ● Edit existing questions.
 ● Add or delete questions.
 ● Import multiple questions using the bulk-paste format.
 ● Restore the default demo questions.

Example bulk-import format:

Q: What does DPG stand for?

A: Digital Programming Group

B: Digital Public Goods

C: Data Protection Guide

D: Digital Product Generation

ANSWER: B

HINT: Open digital resources for public good.

FACT: Certified DPGs help achieve the UN SDGs.

The correct answer must be indicated with ANSWER: A, ANSWER: B, ANSWER: C, or ANSWER: D.

Question changes are automatically saved in the browser’s local storage. They are stored in the browser used to edit them and are not automatically shared with other users or devices.

Technologies Used

 ● HTML5
 ● CSS3
 ● JavaScript
 ● SVG for the illustrated city and mascot
 ● Tailwind CSS (loaded via CDN)
 ● Google Fonts: Fredoka and Inter (loaded via Google Fonts)

Project Structure

.

└── city_clean_up_classroom_quiz_game.html

Data Persistence
The current question editor uses browser local storage for question changes.

The new economy, inventory, decoration placement, mini-game completion, and achievement data should use the existing application storage architecture when implemented. If authentication or a database is introduced, player-specific data should be associated with the current player.

Browser Compatibility

Use a recent version of a modern browser such as Google Chrome, Microsoft Edge, Firefox, or Safari.

License

No license has been specified yet. Add a LICENSE file and update this section if you intend to distribute the project as open source.
