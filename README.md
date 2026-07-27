# Farframe Website

Static multi-page Farframe website prepared for GitHub and Netlify.

## Included routes

- `/` — Home
- `/products/` — Products
- `/about/` — About
- `/contact/` — Contact with Netlify form handling
- `/privacy/` — Privacy notice
- `/thanks/` — Form success page
- `/404.html` — Error page

## Deploy through GitHub and Netlify

1. Create a GitHub repository named `farframe-website`.
2. Upload every file and folder from this package to the repository root.
3. In Netlify, choose **Add new project → Import an existing project**.
4. Connect GitHub and select the repository.
5. Build settings:
   - Build command: leave blank
   - Publish directory: `.`
6. Deploy the site.
7. In Netlify, open **Forms** and confirm that `farframe-contact` was detected.
8. Add an email notification for form submissions.
9. Test the form on the Netlify preview address.
10. Connect `farframe.ca` only after all pages and email DNS records are checked.

## Important replacements before final launch

- Replace `/assets/brand/farframe-symbol.svg` with the approved symbol.
- Replace the temporary typed `FARFRAME` word in the shared header/footer markup with the approved full wordmark asset if desired.
- Add real product screenshots and demonstrations when ready.
- Review the privacy notice for your exact service providers and retention process.
- Self-host IBM Plex font files if you want to remove Google Fonts.

## Netlify form

The form is already configured with:

- `data-netlify="true"`
- hidden `form-name`
- honeypot spam field
- success redirect to `/thanks/`

No JavaScript API key is required for the initial form.
