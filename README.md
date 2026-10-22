# Activity Registration Report → WhatsApp Queue Sender CSV

A **privacy-first, client-side web app** that converts an Activity Registration Report (`.xlsx`) into a CSV ready for the [WhatsApp Queue Sender](https://github.com/antloh-sh/WhatsApp-Sender).

✅ No server · ✅ No database · ✅ No uploads · ✅ Works on GitHub Pages

---

## What it does

1. You upload the `.xlsx` activity member report.
2. The app auto-detects the table header row and the relevant columns (by header name).
3. It extracts each member's **Name** and their **mobile number** (the number tagged `(M)`), prefixes it with the Singapore country code `65`, and builds a CSV.
4. Rows that can't produce a valid mobile number are **skipped** and listed in an on-screen report — which can also be downloaded.

All processing happens in your browser. **Nothing is ever uploaded to a server.**

---

## Output format

The generated contacts CSV matches the format required by the [WhatsApp Queue Sender](https://github.com/antloh-sh/WhatsApp-Sender):

```csv
Name,ContactNumber
ALBERT,6588911900
ANANTHAN,6596693033
