# Synthetic card alerts for "AI Bookkeeper: Capture"

Fake data only. Send each one TO the demo inbox FROM a different address (Gmail often marks mail you send yourself as read, and the trigger only picks up unread mail). The subject must contain "Transaction alert".

## 1. Clear subscription (expect: Approved)
Subject: Transaction alert: card ending 4821
Body:
Demo Bank card alert. Your card ending in 4821 was used on Nov 10, 2026 for USD 54.99 at ADOBE *CREATIVE CLOUD, adobe.com CA. If you did not make this purchase, call us.

## 2. Client lunch (expect: Approved, Meals and Entertainment)
Subject: Transaction alert: card ending 4821
Body:
Demo Bank card alert. Card ending 4821. Amount: $86.40. Merchant: THE CAPITAL GRILLE NYC. Date: 11/11/2026 13:42.

## 3. Unclear marketplace buy (expect: Needs review)
Subject: Transaction alert: card ending 4821
Body:
Demo Bank card alert. A purchase of USD 127.43 was made with your card ending 4821 at AMZN Mktp US*2K4L19XQ2.

## 4. Dedupe test
Run the workflow again on the same 3 emails (mark them unread in Gmail). Expect: no new Airtable rows.
