
---

# 🏢 Dur Muhammad Noonari - Finance & Property Management Pro

A lightweight, high-performance, single-file Web Application designed for comprehensive real estate property management, tenant tracking, automated utility bill splitting, allowance tracking, loan ledgers, and document verification.

Built with **HTML5, Tailwind CSS, Vanilla JavaScript, Chart.js, html2pdf.js, QRCode.js, and Html5-QRCode**.

---

## 🚀 Features

### 📊 1. Visual Analytics & Real-Time Dashboard

* **Dynamic Capacity Occupancy Gauge**: Calculates real-time occupancy rates based on actual property capacity vs. total occupied units:

$$\text{Occupancy Rate} = \left( \frac{\text{Total Occupied Units}}{\text{Total Property Capacity}} \right) \times 100$$


* **Interactive Financial Charts**: Visual breakdowns of Income vs. Expenses (Doughnut Chart) and historical monthly cash flow trends (Line Chart).
* **Automated Smart Insights Engine**:
* Scans pending dues and flags accounts overdue by **>10 days**.
* Performs **Month-over-Month utility comparison** to detect sudden spike percentages in utility bills.
* Alerts when active loan receivables exceed current liquid cash reserves.



### 🏠 2. Property & Tenant Management

* **Flexible Property Units**: Register properties as Single-Family (1 unit capacity) or Shared Units (custom capacity).
* **Tenant Lifecycle Tracking**: Store tenant details, monthly rent agreements, CNIC, permanent address, entry date, and lease milestone end dates.
* **30-Day Automated Lease Renewal Alert**: Auto-calculates lease expiration dates and displays a WhatsApp alert badge when a lease renewal is $\le 30$ days away.

### 🧾 3. Utility Billing & WhatsApp Reminder System

* **Utility Splitting Engine**: Log total utility bills (Electricity/HESCO, Gas/SSGC, Water & Maintenance) and automatically split charges across all property tenants.
* **Itemized WhatsApp Dues Hub**: One-click WhatsApp message builder that formats itemized breakdowns (Rent + Utilities) and calculates total payable dues directly to the tenant's phone number.

### 📄 4. PDF Receipts & Tenancy Agreements with Scannable QR Codes

* **Official Rent & Utility PDF Receipts**: Generates itemized PDF statements showing agreed rent, utility breakdown, total paid, and remaining balance.
* **Residential Tenancy Agreement PDF**: Creates official tenancy legal agreements on demand.
* **Scannable Verification QR Codes**: Embeds rendered QR codes onto both PDF Receipts and Agreemets.

### 🔍 5. Integrated Live QR Code Reader & Document Verifier

* **Camera & File QR Scanner**: Use mobile/desktop webcams or upload an image file to scan any document's QR code.
* **Ledger Registry Matching**: Cross-checks scanned QR tokens against the local system registry to display a **`✓ MATCHED & VERIFIED`** badge or an **`✕ INVALID / UNMATCHED`** security alert.

### 🔎 6. Multi-Criteria Transaction Filtering & Data Backup

* **Advanced Multi-Filter Suite**: Filter transactions simultaneously by Search Keyword, Tenant Name, Category, Minimum/Maximum Amount Range, and Date Range.
* **CSV Export**: Export filtered transaction views directly into standard Excel-compatible `.csv` files.
* **Local Storage & Backup**: Complete JSON export/import capability for offline backup and restoring full app state.
* **Security PIN & Dark Mode**: Protected by a customizable 4-digit manager PIN (`6784`) and local dark mode preference persistence.

---

## 🛠️ Technology Stack

| Component | Library / Framework | Source |
| --- | --- | --- |
| **UI Framework** | Tailwind CSS | Script CDN |
| **Icons & Fonts** | FontAwesome 6 & Plus Jakarta Sans | Google Fonts & cdnjs |
| **Analytics** | Chart.js (`v4.4.0`) | jsDelivr |
| **PDF Export** | `html2pdf.js` (`v0.10.1`) | cdnjs |
| **QR Generator** | `qrcode.js` (`v1.0.0`) | cdnjs |
| **QR Reader** | `html5-qrcode` (`v2.3.8`) | Unpkg |

---

## 📦 Installation & Setup

Because the application is built as a **Self-Contained Client-Side Web App**, no complex server runtime or Node.js environment is required to run it.

1. **Clone or Download the repository**:
```bash
git clone https://github.com/your-username/noonari-finance-pro.git
cd noonari-finance-pro

```


2. **Open the application**:
Simply double-click `index.html` or open it in any modern browser (Chrome, Edge, Firefox, Safari).
3. **Login Access**:
* **Default PIN**: `6784`



---

## 🔧 Production Build Recommendations

If you plan to deploy this project to a production web server (e.g., Vercel, Netlify, GitHub Pages, or Hostinger), consider the following best practices:

1. **Tailwind CSS Compilation**:
Instead of relying on the browser-side Tailwind CDN script, compile Tailwind using the CLI:
```bash
npx tailwindcss -i ./src/input.css -o ./dist/output.css --minify

```


2. **Offline Local Storage**:
Data is stored securely in your browser's `localStorage` (`noonari_family_pro_data_v7`). Remember to regularly use the **Backup Data** button in the sidebar to download standard `.json` backups of your ledger.

---

## 📜 License

Distributed under the **MIT License**. Free for personal and commercial property management use.
