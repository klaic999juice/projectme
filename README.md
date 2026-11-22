# Miss Luther

A small storefront prototype for listing products and collecting preorder requests. The landing-page name and headline letters have entrance animations, with reduced-motion support.

## Try it

1. Deploy this repository to Vercel. No build command is required.
2. Select **Create account**. The first account created in that browser becomes the shop admin.
3. Open **Dashboard** to add/edit/hide products and review preorder requests.
4. Shoppers can reserve a quantity and leave their name, email, optional phone number, and a note.

The storefront displays and accepts prices in Ghanaian cedis (GHS). Use the header control to switch between dark and light themes.

## Demo limitation

Accounts, roles, listings, and preorder requests use browser `localStorage` only. This is not production authentication or a shared inventory system. Before collecting real customer data, connect a secure backend with server-enforced authorization and a database.
