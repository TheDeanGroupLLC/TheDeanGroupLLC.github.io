# Contact Form Setup Instructions

The contact form in `contact.html` is currently static HTML. To make it send messages to `Andelyn@TheDeanGroup.llc`, connect it to a form handling service.

## Option 1: Web3Forms

Good for a static site because it does not require a backend.

1. Go to Web3Forms and create an access key for the email address that should receive submissions.
2. In `contact.html`, find the opening form tag:

```html
<form>
```

3. Replace it with:

```html
<form action="https://api.web3forms.com/submit" method="POST">
  <input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">
```

4. Find the submit button. It currently uses:

```html
<button type="button"
```

5. Change it to:

```html
<button type="submit"
```

6. Test the form after deployment.

## Option 2: Formspree

Another simple option for static websites.

1. Create a Formspree form endpoint.
2. Replace the opening form tag with:

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

3. Change the submit button from `type="button"` to `type="submit"`.
4. Submit a test message and confirm delivery.

## Option 3: Netlify Forms

Use this only if the site is hosted on Netlify.

1. Replace the opening form tag with:

```html
<form name="contact" method="POST" data-netlify="true">
  <input type="hidden" name="form-name" value="contact">
```

2. Change the submit button from `type="button"` to `type="submit"`.
3. Deploy to Netlify.
4. Test the form in production.

## Calendly Buttons

The separate Calendly placeholder section has been removed.

To add Calendly, update the two button links inside the “Three Contact Options” section:

```html
<a class="btn btn-secondary" href="#calendly-scoping">Book a Call</a>
```

and

```html
<a class="btn btn-secondary" href="#calendly-office-hours">Book Office Hours</a>
```

Replace the `href` values with the actual Calendly event URLs.
