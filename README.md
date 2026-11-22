# Goodfinds

A small storefront prototype for listing products and collecting preorder requests. It is a dependency-free static website that can be hosted on GitHub Pages.

## Try it

1. Open `index.html` from a local web server or deploy the repository with GitHub Pages (HTTPS is needed for account creation).
2. Select **Create account**. The first account created in that browser becomes the shop admin.
3. Open **Dashboard** to add/edit/hide products and review preorder requests.
4. Sign out and create another account (or use another browser profile) to try the shopper flow. Customers can reserve a quantity and leave their name, email, optional phone number, and a note.

The starter catalog is sample data. Listing, account, and preorder data are saved in that browser's `localStorage`; no information is sent to a server. Preorders are requests, not payments or confirmed orders.

## Important before using this for a real shop

This is a UI prototype, **not production authentication or a production preorder system**. Browser storage can be read, edited, or deleted by the person using the browser. The first-account-admin rule is only enforced independently in each browser, so it does not securely establish a global first admin. Product inventory and customer requests are not shared across shoppers or devices. Passwords are hashed in-browser for the demo, but client-side roles and local data are not an access-control boundary. Do not use real or reused passwords, and do not collect real customer contact information with this prototype.

Before launch, connect a backend with server-enforced authentication/authorization and a database; provision the initial admin through a trusted one-time setup; validate stock and requests on the server; and add appropriate privacy, retention, and customer-data protections. Never rely on a role stored in browser state to authorize admin actions.

## Deploy with GitHub Pages

In the repository, open **Settings → Pages**, choose the `main` branch and `/ (root)` as the publishing source, and save. Once published, use the HTTPS URL provided by GitHub Pages.
