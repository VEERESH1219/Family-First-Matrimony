# 🏡 Family-First Matrimony Platform

A secure, traditional, family-oriented matrimony web application built to support
**verified, privacy-first, and family-controlled matchmaking**.

This platform is designed specifically for Indian matrimonial culture where
**families play the central role**, not individuals.

---

## 🎯 Core Philosophy

> Marriage is a union of families, not just individuals.

Unlike modern matrimony or dating platforms, this system strictly enforces:
- Family involvement
- Identity and caste verification
- Privacy protection (especially for women)
- Zero direct male–female interaction

---

## 👤 User Roles

### Bride / Groom (Profile Owner)
- Signs up and creates a profile
- Uploads photos and verification documents
- Cannot browse profiles
- Cannot chat with anyone

### Family (Decision Maker)
- Browses verified profiles
- Sees only same-caste profiles
- Sends and receives connection requests
- Communicates only with other families

### Admin (Gatekeeper)
- Verifies Aadhaar and caste certificates
- Approves or rejects profiles
- Controls profile visibility and photo access

---

## 🔞 Age Eligibility Rules

- **Women:** 18 years and above
- **Men:** 21 years and above

Age is validated using Aadhaar.
Users below the minimum age are automatically rejected.

---

## 🖼️ Photo Privacy Policy

- Women photos are **private by default**
- Men photos are hidden until verification
- Photos remain locked until:
  - Profile completion
  - Aadhaar verification
  - Caste verification
  - Admin approval

---

## 🪪 Aadhaar Verification

- Mandatory for all users
- Used only for:
  - Age validation
  - Identity verification
- Aadhaar data is encrypted and never shared

---

## 🧾 Caste Certificate Verification

- Mandatory caste certificate upload
- Manually verified by admin
- Profiles are visible **only within the same caste**
- Cross-caste browsing is not allowed

---

## 🔄 Matchmaking Flow

1. User signs up and completes profile
2. Photos and documents are uploaded
3. Admin verifies Aadhaar and caste
4. Profile becomes fully verified
5. Families browse same-caste profiles
6. Connection requests are exchanged
7. Family-to-family communication starts
8. Marriage decision happens offline

---

## 🚫 Platform Restrictions

- No unverified profiles in search
- No direct chat between men and women
- No photo visibility without admin approval
- No matchmaking without caste verification

---

## 🛠️ Technology Stack

- Frontend: React
- Backend: Node.js + Express
- Database: PostgreSQL
- Authentication: JWT
- Storage: AWS S3
- Deployment: Docker

---

## 📄 License

MIT License
