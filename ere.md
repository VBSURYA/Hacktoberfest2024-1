## 🔎 Daily Overview
Today was all about cleaning and tightening the **Sabbkuh (sabbkuch.in)** store.  
* Removed endless duplicate products that were created by the CSV import.  
* Fixed pricing for the affected SKUs and confirmed GST‑inclusive totals.  
* Resolved the double‑tax issue by switching to the “prices include tax” setting.  
* Planned the domain switch to Shopify for tomorrow.

---

## 📌 Step‑by‑Step Breakdown

| # | Task | Outcome | Comment |
|---|------|---------|---------|
| **1️⃣** | **Import pricing sheet & detect duplicates** | ✅ Duplicates identified on CSV upload | Duplicate product creation persisted after first removal attempt. |
| **2️⃣** | **Remove duplicates & verify uniqueness** | ✅ All duplicates eliminated | Re‑imported with unique IDs; no repeats appear in admin. |
| **3️⃣** | **Manually correct pricing** | ✅ Prices updated | GST already included – no extra charges set in Shopify tax. |
| **4️⃣** | **Replace default all produt collection image** | ✅ New images uploaded | Client supplied high‑res photos;  |
| **5️⃣** | **Audit tax configuration** | ✅ No “extra tax” applied | Set store to “prices include tax”; test transaction confirmed correct total. |
| **6️⃣** | **Domain migration prep** | ⚙️ DNS plan drafted | Detailed A, AAAA, and CNAME entries ready for tomorrow’s deployment. |

---

## 📈 Next‑Day Tasks (Tomorrow)

1. **Push live to Sabbkuh domain**  
   *Log in to registrar ➜ DNS Settings ➜ Update/Add records:*
   - **A Record**  
     - Type: **A**  
     - Host/Name: **@**  
     - Points to: **23.227.38.65**  
     - TTL: Default (or 1 hr)
   - **AAAA Record** (if supported)  
     - Type: **AAAA**  
     - Host/Name: **@**  
     - Points to: **2620:0127:f00f:5::**  
     - TTL: Default
   - **CNAME Record**  
     - Type: **CNAME**  
     - Host/Name: **www**  
     - Points to: **shops.myshopify.com.**  
     - TTL: Default

2. **Verify DNS propagation**  
   - Use `dig` / `nslookup` and Shopify diagnostics.  
   - Confirm SSL/TLS issuance and correct mapping of `sabbkuch.in` & `www.sabbkuch.in`.

3. **Post‑Go‑Live QA**  
   - Full‑stack functional test: catalogue, cart, checkout, admin dashboard.  
   - Mobile responsiveness check on iOS/Android.  
   - Monitor transaction logs for any lingering tax or pricing anomalies.

---

### ✅ Ready Deliverables Today
- Duplicate‑free product list  
- GST‑included pricing confirmed  
- Product images replaced  
- Tax settings verified  
