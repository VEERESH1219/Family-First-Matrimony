# ⚙️ System Specification – Family-First Matrimony Platform

## 1. User Authentication
- JWT-based authentication
- Role-based access (User, Family, Admin)
- Secure password hashing

---

## 2. Profile Specification

### Profile Fields
- Name
- Date of Birth
- Gender
- Education
- Occupation
- Location

Each user can have only one profile.

---

## 3. Document Specification

### Supported Documents
- Aadhaar Card (mandatory)
- Caste Certificate (mandatory)

### Rules
- Documents must be approved by admin
- Unverified documents block profile visibility

---

## 4. Photo Specification

- Multiple photo uploads allowed
- Photos remain locked until admin approval
- Women photos are private by default

---

## 5. Caste Verification Logic

- One verified caste per profile
- Same-caste visibility enforced at query level
- Unverified caste profiles are excluded from search results

---

## 6. Matchmaking Rules

- Profiles visible only after full verification
- Families initiate and accept connections
- Communication enabled only after mutual approval

---

## 7. Admin Specification

### Admin Capabilities
- View pending verifications
- Approve or reject documents
- Lock or unlock profile visibility
- Moderate profiles

---

## 8. Security Specifications

- Encrypted Aadhaar storage
- Secure file storage (AWS S3)
- Role-based API protection
- Audit logging for admin actions

---

## 9. System Constraints

- No direct interaction between men and women
- No access to profiles without verification
- No matchmaking outside defined caste rules
