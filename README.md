# pines-wedding-plan
# Emerald Pines Country Club Wedding Planner

A static, front-end wedding planning demo rebuilt from the supplied project as four files: `index.html`, `styles.css`, `app.js`, and `README.md`. It uses plain HTML, CSS, and JavaScript, so you do not need React, Node.js, or a package install to view it.

## Run it in Visual Studio Code

1. Download and unzip the project.
2. In Visual Studio Code, choose **File → Open Folder** and select `emerald-pines-wedding-planner`.
3. Open `index.html` and use **Live Server → Open with Live Server**. If Live Server is not installed, open the Extensions panel and install **Live Server**.
4. You can also open `index.html` directly in a browser. For a local server, open the VS Code terminal in the project folder and run `python3 -m http.server 8000`, then visit `http://localhost:8000`.

## Demo sign-in

The demo accepts any email and password. Select a role card to fill the example account details.

| Role | Email | Password |
| --- | --- | --- |
| Wedding Client | `amelia.caldwell@example.com` | `demo1234` |
| Coordinator | `elena.rhodes@emeraldpines.club` | `demo1234` |
| Administrator | `yasmin.park@emeraldpines.club` | `demo1234` |

Use the **View as** control to switch roles after sign-in. The **Presentation** menu includes example requests and simulated payment/refund outcomes.

## Included flows

- Client: home, venue availability, wedding plan form, review, simulated refundable $100 application fee, request status, receipt, and help/inquiries.
- Coordinator: dashboard, request queue, requirement review, approve/revise/cannot-fulfil decisions, venue closures, refunds, and help.
- Administrator: dashboard, staff account list, add/edit/deactivate staff, and help.
- Sample data: requests EP-10241 through EP-10244 and DRAFT-01, four venues, staff, closures, and an inquiry.

This is a front-end demo. It has no server, database, real payment processor, email or text delivery. Demo changes live in memory and reset when the page refreshes. Use **Presentation → Reset demo data** to restore the original sample records without refreshing.

## Publish the project to GitHub

### Option A: GitHub website

1. Sign in at [GitHub](https://github.com/) and choose **New repository**.
2. Enter a repository name such as `emerald-pines-wedding-planner`. Choose Public or Private, then create it.
3. In the new repository, choose **Add file → Upload files**.
4. Drag the four project files into the upload area. Commit the changes.

### Option B: Git in the VS Code terminal

Create an empty repository on GitHub first. Then, from the project folder, run:

```bash
git init
git add index.html styles.css app.js README.md
git commit -m "Add Emerald Pines wedding planner demo"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/emerald-pines-wedding-planner.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username. If Git asks you to sign in, follow the prompt in your browser.

## Publish a live demo with GitHub Pages

1. Open the repository on GitHub and select **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch `main` and folder `/ (root)`, then save.
4. Wait for the Pages link to appear in that section. Open it to view the site.

The app uses hash-based routes (for example, `/#/status`), which work with GitHub Pages without extra server configuration.
