# PolicySnap Privacy Policy

**Effective date:** July 13, 2026  
**Last updated:** July 13, 2026

PolicySnap (“we,” “our,” or “the Extension”) is a Chrome browser extension that helps people understand insurance policy language using artificial intelligence (AI). This Privacy Policy describes what information is processed when you use PolicySnap, how it is used, and the choices you have.

**Contact:** For privacy questions, contact the developer through the Chrome Web Store listing for PolicySnap or the PolicySnap GitHub organization (PolicySnapAdmin).

---

## 1. Summary

| Topic | What happens |
|--------|----------------|
| Account | No PolicySnap account is required |
| Free summaries | Policy text is sent to **PolicySnap’s secure backend**, then to **OpenAI** to generate a summary |
| Unlimited mode | If you add your own OpenAI API key, policy text is sent **from your browser to OpenAI** using your key; we do not receive that key |
| Local device | History, settings, theme colors, free-usage cache, and optional API key are stored in **Chrome local storage** on your device |
| Selling data | We do **not** sell your personal information or insurance content |

---

## 2. Information stored on your device

PolicySnap uses Chrome’s `storage.local` API. This data stays on your device unless you clear it or uninstall the extension. It may include:

- **Analysis history** — short labels for past requests and the AI summaries you generated  
- **Optional OpenAI API key** — only if you choose to enter one in Settings (stored locally; not uploaded to PolicySnap)  
- **Install identifier** — a random ID generated on your device so free monthly limits can be enforced fairly  
- **Free-usage cache** — an approximate remaining free count for the current month (for display in the UI)  
- **Theme / color preferences** — app appearance settings you choose  

We do **not** access your browsing history, other websites’ content, or your Google account through PolicySnap.

---

## 3. Information processed when you run a summary

When you paste policy text or upload a policy PDF and request a summary, the **text content you submit** is processed to generate a response.

### 3.1 Free tier (default)

1. Extracted or pasted text is sent from the Extension to **PolicySnap’s backend** (hosted on **Supabase** infrastructure).  
2. The backend sends that text to **OpenAI** to generate the summary.  
3. The summary is returned to the Extension and may be saved in your local history.  
4. To enforce free limits, the backend records **usage counts** tied to your install identifier and a **hashed** network signal (for example, a hash related to IP address). We use this to prevent abuse of the free tier — not to build advertising profiles.

We do **not** intend to keep full policy documents as a permanent content archive on our servers. Usage counters and technical logs needed to operate and secure the service may be retained for a limited operational period.

### 3.2 Unlimited mode (your own OpenAI API key)

If you enable your own OpenAI API key in Settings:

- Submitted text is sent **directly from your browser to OpenAI**.  
- PolicySnap does **not** receive or store that key on our servers.  
- OpenAI’s processing and retention rules apply under their terms and privacy policy.

### 3.3 PDF uploads

PDF processing (text extraction) happens **in your browser**. Only the extracted text that is sent for analysis follows the free-tier or own-key path described above. Scanned/image-only PDFs may not extract text successfully.

---

## 4. How we use information

We use the information described above to:

- Provide AI summaries and key-point explanations  
- Enforce free monthly limits and reduce abuse  
- Remember your history and settings on your device  
- Operate, secure, and improve the reliability of the free-tier backend  

We do **not** use your insurance text to sell ads or to train a public model under PolicySnap’s control. OpenAI processes content under their own policies when you use either free tier (via our backend) or your own key.

---

## 5. Third-party services

### OpenAI  
Generates summaries. When free tier is used, OpenAI receives the text from our backend. When you use your own key, OpenAI receives the text from your browser.  
Privacy policy: [https://openai.com/policies/privacy-policy](https://openai.com/policies/privacy-policy)

### Supabase  
Hosts PolicySnap’s free-tier backend (Edge Functions and related database tables for usage limits).  
Privacy policy: [https://supabase.com/privacy](https://supabase.com/privacy)

### Google / Chrome Web Store  
Distributes the Extension. Google’s terms and privacy policies apply to store installation and updates.

**Payments:** PolicySnap’s free tier does not require payment. If paid upgrades or payment processors are added later, this policy will be updated before those features process payment data.

---

## 6. Data retention

| Data | Retention |
|------|-----------|
| Local history, settings, optional API key | Until you clear Chrome storage or remove the Extension |
| Free-tier usage counters (install / IP hash) | Kept as needed to enforce monthly limits (typically aligned with calendar months and operational needs) |
| Transient processing of submitted text | Processed to produce a summary; not intended as a long-term document library on our servers |

---

## 7. Your choices and rights

You can:

- **Stop using free tier** and switch to your own OpenAI key in Settings  
- **Remove your API key** from the Extension at any time  
- **Clear local data** via Chrome settings or by uninstalling PolicySnap  
- **Uninstall** the Extension from `chrome://extensions`  
- Limit what you submit — only paste or upload content you are comfortable sending for AI analysis  

Depending on where you live, you may have additional rights under applicable privacy laws (for example, access or deletion requests). Contact us using the methods above and we will respond as required by law.

---

## 8. Children’s privacy

PolicySnap is not directed to children under 13, and we do not knowingly collect personal information from children under 13. If you believe a child has provided such information through the Extension, contact us and we will take appropriate steps.

---

## 9. Security

We take reasonable measures appropriate to a small software product, including:

- Keeping the free-tier **OpenAI API key on the server**, not inside the Extension package  
- Restricting free-tier database tables with access controls so clients cannot freely rewrite quotas  
- Using HTTPS for network requests  

No method of transmission or storage is 100% secure. Please do not submit secrets (passwords, full government ID numbers, etc.) in policy text unless necessary for your own understanding of a document you already possess.

---

## 10. International processing

Our backend and third-party providers (including OpenAI and Supabase) may process data in the United States or other countries. By using PolicySnap, you understand that information may be transferred to and processed in jurisdictions that may have different data-protection rules than your own.

---

## 11. Not legal advice

PolicySnap provides **informational** plain-language explanations of insurance text. It is **not** legal advice, insurance advice, or a substitute for reading your full policy or consulting a licensed professional. AI output can be incomplete or incorrect.

---

## 12. Changes to this policy

We may update this Privacy Policy from time to time. The “Last updated” date at the top will change when we do. Material changes may also be noted in the Chrome Web Store listing or on our website. Continued use of PolicySnap after an update means you accept the revised policy.

---

## 13. Website

Our public website and this policy may be published at:

- https://policysnapadmin.github.io/PolicySnap/  
- https://policysnapadmin.github.io/PolicySnap/Privacy.md  
- https://raw.githubusercontent.com/PolicySnapAdmin/PolicySnap/main/Privacy.md  

If URLs change, the Chrome Web Store listing will point to the current privacy policy location.
