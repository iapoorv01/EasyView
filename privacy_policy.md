# EasyView Extension Privacy Policy

## 🔒 Privacy-First Approach

EasyView is designed with your privacy as the top priority. We implement a strict separation between sensitive data and user preferences.

> **Note:** For our full, legally binding Privacy Policy regarding your EasyView Account, Premium Subscriptions, and Website interactions, please read the [Official EasyView Privacy Policy](https://easyview.in/privacy-policy).

## Extension Data Storage

### **Local-Only Storage (Bring Your Own Key)**
If you choose to use the "Bring Your Own Key" (BYOK) feature instead of our built-in Premium quotas, your Google Gemini or OpenRouter API key is stored using `chrome.storage.local`. This means it:
- ✅ **Never syncs** to any cloud service
- ✅ **Device-only** - stays on your computer
- ✅ **No transmission** - never leaves your device to our servers

### **Sync Storage (Settings & Premium Status)**
User preferences (feature toggles, visual settings) and your securely hashed Premium Status are stored using `chrome.storage.sync`, which:
- ✅ Syncs across your Chrome browsers
- ✅ Includes basic account metadata (email) if you are logged in
- ✅ Does **NOT** include custom API keys

## Premium Authentication & AI Processing

With the launch of **EasyView Premium**, we use **Supabase** for secure backend validation.

- **Free / Premium Tier (Built-in):** If you use our built-in AI quotas, your browser securely authenticates with our backend using a signed token. We **do not log or store** the text you highlight. The text is immediately passed to the AI provider and discarded.
- **BYOK Tier:** If you provide your own API key, your browser communicates **directly** with the AI provider (Google or OpenRouter). This communication bypasses our servers entirely.

## What We Collect (Via Supabase)
If you create an account, we securely collect:
- Your Email Address (via OAuth)
- Subscription Payment Status (via Stripe/Razorpay)
- Anonymous Usage Analytics (e.g., "Jargon Decoder Used", no page text is saved)

**We NEVER collect:**
- Your browsing history or exact URLs
- Your personal API keys
- The text you highlight to read or decode

## Your Control
You have complete control over your data:
1. **API Key**: Delete it from the Settings UI at any time.
2. **Account Deletion**: Contact support at easyview.support@gmail.com to permanently delete your account and all associated data under GDPR/CCPA.
3. **Uninstall**: Uninstalling the extension completely wipes all locally cached settings.

---

**Last Updated:** May 2026  
**Privacy Guarantee:** We will never sell, share, or monetize your personal data. Period.
