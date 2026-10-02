## Microsoft Entra ID — Identities & Authentication Cheat Sheet

### Identity Types
| Type | Represents | Managed By |
|---|---|---|
| User | Human employee/guest | Admin/self |
| Group | Collection of users/devices | Admin |
| Device | Registered/joined endpoint | Admin/Intune |
| Service Principal | App/service identity | Developer (manual creds) |
| Managed Identity | App/service identity | Azure (auto creds) |

### MFA vs Passwordless
| Category | Methods |
|---|---|
| MFA (password + factor) | Microsoft Authenticator (push/OTP), SMS, Voice call, OATH hardware token, OATH software token |
| Passwordless (no password) | Windows Hello for Business, FIDO2 security key, Microsoft Authenticator (phone sign-in) |

**Exam note:** Passwordless methods remove the password entirely; MFA methods add a second factor *to* a password.

### SSPR Key Facts
- Default **2 methods required** to reset (configurable to 1 or 2).
- Free tier: cloud-only unlock only. **P1/P2 required** for full SSPR + on-prem password writeback.
- Combined registration lets one setup cover both MFA and SSPR methods.

**Common mistake:** Choosing Conditional Access or PIM for "users reset own password" scenarios — neither handles password reset.

### External Identities
| Scenario | Solution |
|---|---|
| Partner org needs access to internal resource | **B2B collaboration** (guest invite) |
| Consumer-facing app, social login (Google/Facebook) | **External ID for customers (B2C)** |
| On-prem AD needs to sync/federate with cloud | **Entra Connect** (PHS / PTA / AD FS federation) |

### Federation/Sync Options (Entra Connect)
| Method | Description | Password stored in cloud? |
|---|---|---|
| Password Hash Sync (PHS) | Hash of password hash synced to cloud | Yes (hashed) |
| Pass-through Authentication (PTA) | Validation happens on-prem via agent | No |
| Federation (AD FS) | On-prem AD FS issues tokens | No |

**Exam note:** PHS is simplest and most resilient (works even if on-prem is down, if cached); AD FS adds infrastructure and complexity — used for advanced scenarios like smart-card auth.

### FIDO2 vs Windows Hello for Business
| Feature | FIDO2 | Windows Hello for Business |
|---|---|---|
| Portable across devices | Yes (USB/NFC/BT key) | No (bound to device) |
| Auth factor | Key + PIN/biometric on key | Biometric/PIN + TPM on device |

**Common mistake:** Confusing service principal (manual credential management) with managed identity (Azure auto-manages credentials) — the 'no stored secrets' clue always points to managed identity.
