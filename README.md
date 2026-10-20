# G Works - Doors and Windows

A responsive landing page concept for a windows and doors business. It includes product sections, an overview of the installation process, and a contact call-to-action. The Windows and Doors cards open `windows.html` and `doors.html` in new tabs with style examples and descriptions. Project calls-to-action open `order.html` with a simple order-request form.

## Run

Install the development dependency and start the local server:

```powershell
npm install
npm run dev
```

Vite opens `Web app testing.html` and reloads the page as you edit. You can still open the HTML file directly in a browser. The photography and Russo One font load from online sources, so an internet connection is needed for them.

## Preview on a phone

Connect the phone and computer to the same Wi-Fi network, run `npm run dev`, and open the `Network` URL Vite prints in the terminal. Allow Node.js through Windows Firewall on private networks if prompted. This shares the preview only on your local network.

## Public deployment with GitHub Pages

The GitHub Actions workflow in `.github/workflows/deploy.yml` publishes the static HTML and SVG files whenever changes are pushed to the `main` branch. The root `index.html` redirects visitors to the landing page.

To publish, create a **public** GitHub repository, push these project files to its `main` branch, and set the repository's **Settings → Pages → Build and deployment → Source** to **GitHub Actions**. The workflow will deploy the site; its public URL will appear in the repository's Pages settings and in the workflow run.

The site stays available while the repository, GitHub Pages, and the account remain active; no hosting service can guarantee it will exist forever. Everything in the site is public, including the placeholder `hello@gworks.example` address. The order form only prepares an email draft and does not receive or store orders.

## Before publishing

Replace the sample `hello@gworks.example` contact address in `order.html` with the business's real email when ready. The order form prepares an email draft; it does not store or process orders on a server.
