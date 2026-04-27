# Invoicer

Invoicer helps you build a simple invoice, preview it, and download it as a PDF.

Use it when you need to create a freelance or small-business invoice without rebuilding the same details from scratch every time.

## Quick Start

1. Enter your user key.
2. If you have a previous PDF made by this app, upload it to pre-fill details.
3. Check or enter your details.
4. Enter the client details.
5. Add the invoice number, invoice date, line items, currency, tax, and payment terms.
6. Choose the payment methods and payment details to show.
7. Preview the invoice.
8. Download the PDF.
9. Open the downloaded PDF and check it before sending it.

## Restoring From A Previous Invoice

PDFs made by Invoicer contain hidden restore data. If you upload one of those PDFs, the app can use it to pre-fill a new invoice.

This is there to save typing, not to remove checking. Always review:

- invoice number
- invoice date
- client name and address
- line items
- rates and quantities
- tax label and tax rate
- payment terms
- payment details
- final total

If the uploaded PDF was not made by Invoicer, or if the restore data is missing, just continue manually.

## Payment Terms

For ordinary calendar-day terms, enter a number:

```text
30
```

For business-day terms, use `Net-`:

```text
Net-30
```

Business-day calculations may account for supported public holidays where available. Still check the due date yourself.

## Line Items

Add one line item at a time. Check the description, quantity, rate, and billing basis before adding it.

If something looks wrong in the preview, go back and fix the field before downloading the PDF.

## Payment Details

Only tick payment methods that should appear on this invoice.

If you include bank, Wise, Stripe, or PayPal details, check them carefully in the preview. The app will create the PDF from what is entered.

## What You Get

Invoicer exports a PDF invoice. The filename is based on the invoice number and recipient where possible.

The PDF may also contain restore data so that a future invoice can be pre-filled from it.

## Safe Working Habit

1. Download the PDF.
2. Open it locally.
3. Check every number and payment detail.
4. Save your own copy somewhere sensible.
5. Only then send it to the client.

## If Something Goes Wrong

- If a previous PDF does not restore, enter the details manually.
- If the total looks wrong, check every line item, tax rate, and paid/credit option.
- If the due date looks wrong, check the payment terms field.
- If the wrong payment details appear, go back to Payment Options and untick anything that should not be shown.

## What Invoicer Is Not

Invoicer is not accounting software and does not provide tax, legal, or accounting advice. You are responsible for checking invoice numbers, dates, totals, tax handling, client details, and payment details before sending an invoice.
