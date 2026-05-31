# GRAMPY'S NOTIFICATION API
A simple, custom doors notification API.

# HOW TO USE

Step 1 : Load the API
Execute the main script first. This sets up the notification system and makes it available globally.

Step 2 : 
Open a new tab in your executor and run:
_G.Notify("Title", "Message", "type", duration, font)

# PARAMETERS

"Title"  the bold header of the notification
"Message"  the smaller description below
"type"  controls the color theme: info, warn, error, success, item
duration  how long it stays on screen in seconds (default: 4)
font (optional)  custom font, e.g. Font.fromName("Bangers")

Examples:
lua_G.Notify("Rush incoming", "Ambush is approaching", "warn", 4)
_G.Notify("Item found", "You picked up the key", "item", 5)
_G.Notify("You died", "Caught by Figure", "error", 3)
_G.Notify("Escaped", "You survived Rush", "success", 4)
_G.Notify("Tip", "Stay in the light to avoid Screech", "info", 4)

With a custom font
_G.Notify("Rare item", "Crucifix obtained", "item", 5, Font.fromName("Bangers"))

⚠️ Always execute the main script before running any _G.Notify call, otherwise it won't work.
