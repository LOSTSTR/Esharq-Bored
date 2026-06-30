# Esharq Custom badges (مخصّص)

Custom badges for **specific members** who don't fit the donor / contributor / developer
tiers. Each member gets their own round image with a spinning **RGB (rainbow) ring**, shown
in their profile.

## How to add a member
1. Drop the member's image in this folder, e.g. `custom/<name>.png`
   (square, transparent, 256×256 — it is shown as a circle).
2. Add an entry to `custom.json` mapping the member's Discord user ID to the raw image URL:

   ```json
   {
     "123456789012345678": "https://raw.githubusercontent.com/LOSTSTR/Esharq-Bored/main/badges/custom/<name>.png"
   }
   ```

That member then shows the round image with the RGB ring in their profile.

> The RGB ring design lives in the Esharq client (`esharqBadges.css` → `.esharq-custom-badge`).
> The badge tooltip is currently a shared "مخصّص · Esharq Custom" for everyone.
