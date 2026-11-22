# Goodfinds

A small storefront prototype for listing products and collecting preorder requests. It is a dependency-free static website that can be hosted on Vercel.

## Try it

1. Deploy this repository to Vercel. No build command is required; the site is served from `index.html`.
2. Select **Create account**. The first account created in that browser becomes the shop admin.
3. Open **Dashboard** to add/edit/hide products and review preorder requests.
4. Shoppers can reserve a quantity and leave their name, email, optional phone number, and a note.

The storefront displays and accepts prices in Ghanaian cedis (GHS). Use the dark/light control in the header to switch themes; your choice is saved in that browser. Listing, account, and preorder data are also saved only in the browser's `localStorage`; no information is sent to a server. Preorders are requests, not payments or confirmed orders.

## Important before using this for a real shop

This is a UI prototype, **not production authentication or a production preorder system**. Browser storage can be read, edited, or deleted by the person using the browser. The first-account-admin rule is only enforced independently in each browser, so it does not securely establish a global first admin. Product inventory and customer requests are not shared across shoppers or devices. Passwords are hashed in-browser for the demo, but client-side roles and local data are not an access-control boundary. Do not use real or reused passwords, and do not collect real customer contact information with this prototype.

Before launch, connect a backend with server-enforced authentication/authorization and a database; provision the initial admin through a trusted one-time setup; validate stock and requests on the server; and add appropriate privacy, retention, and customer-data protections. Never rely on a role stored in browser state to authorize admin actions.

## Deploy on Vercel

Import `klaic999juice/projectme` in Vercel. For a static HTML site, choose the **Other** framework preset, leave the build command empty, and use the repository root as the output directory. Future pushes to the connected GitHub branch trigger deployments automatically. If this repository is not connected to a Vercel project yet, create that connection from the Vercel dashboard.
