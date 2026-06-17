
---

## env-variables.md

```md
# Environment Variables

## Purpose

Store secrets and configuration.

---

## Create File

 text
.env.local 
Example
DATABASE_URL=postgresql://...
NEXT_PUBLIC_API_URL=https://api.example.com
Access Server Variable
process.env.DATABASE_URL
Access Client Variable
process.env.NEXT_PUBLIC_API_URL
Security Rule
NEXT_PUBLIC_* = Browser Access

Without NEXT_PUBLIC_* = Server Only
Summary (Hinglish)

Secret keys .env.local me rakhte hain.

NEXT_PUBLIC variables browser me available hote hain.

Database URLs aur API keys kabhi GitHub par push nahi karni chahiye. 
