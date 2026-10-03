# Application for Employment – Online Form

Digital version of form **HESB-SOP-HC-01-F01** (Application for Employment).

## Deploy on GitHub Pages
1. Create a new repository on GitHub and upload `index.html` and this `README.md`.
2. Go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. After a minute your form is live at `https://<your-username>.github.io/<repo-name>/`.

## Submissions go straight to email
Submissions are sent by email through FormSubmit (formsubmit.co), which is free and needs no account.

1. Open `index.html`, find `const HR_EMAIL = "hr@yourcompany.com";` near the bottom, and replace it with your HR email.
2. Deploy, open the live page, and submit one test application.
3. FormSubmit emails an **activation link** to that address. Click it once.
4. From then on, every submission arrives in that inbox as a table. The subject line is *"Job Application: <Name> – <Post>"*, and hitting Reply goes to the applicant.

Optional: after activation, FormSubmit provides a random alias string. Use it in place of the real email so the address isn't visible in the page source.

## Notes
- This form collects sensitive personal data (NRIC, address, health info). Use an HTTPS endpoint you control and handle the data in line with the PDPA 2010.
- To add the company logo, place `logo.png` in the repo and replace the `.brand` block with `<img src="logo.png" alt="HICOM Engineering" height="80">`.
