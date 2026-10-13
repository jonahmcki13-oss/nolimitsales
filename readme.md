# DME Fiber Recruiting Website

## Included
- Responsive black / white / electric-blue recruiting landing page
- Application form: full name, phone number, email
- Client-side validation and spam honeypot
- CRM webhook integration point
- Accurate, qualified compensation and housing language

## Important: CRM is not connected yet
The website cannot deliver leads into your CRM until you provide/configure its lead form endpoint or webhook.

1. In your CRM, create a lead capture form or automation/webhook that accepts an HTTPS POST with JSON.
2. Configure it to map `fullName`, `phone`, `email`, `source`, and `submittedAt` to the correct CRM fields.
3. Open `index.html` and replace the empty value in:
   `window.DME_CRM_WEBHOOK = "";`
   with the CRM's HTTPS endpoint.
4. Make sure the endpoint supports requests from your published website origin (CORS). If your CRM requires a private API key, do not place that key in this HTML. Use a server-side function or trusted automation service instead.
5. Deploy the `index.html` file using a static host such as Netlify, Vercel, or GitHub Pages.
6. Test a dummy lead and confirm it appears in the CRM before sharing the URL.

## Compensation wording
The page says the current plan discussed for some roles starts around $200 per deal, with terms to be confirmed. Verify the actual current written commission plan and employment/contractor status before publishing. Do not advertise guaranteed earnings.

## Privacy
Only collect the fields you need. Add the organization's accurate privacy notice/contact details before public launch if required. Do not collect sensitive personal information in this form.
