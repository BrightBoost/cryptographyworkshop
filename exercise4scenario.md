# “Which Algorithm Should I Use?” Design Scenarios

Let's use applied reasoning.

---

## Scenario A — The Secret Diary App

You’re building a diary app.
Users store personal notes on their phone.
If the phone is stolen, you want the diary unreadable.

Questions:

1. Symmetric or asymmetric?
2. Which algorithm?
3. Where does the key come from?
4. How do you protect the key?

---

## Scenario B — Sending secure messages between two strangers

Alice wants to send an encrypted message to Bob, but they’ve never met.

Questions:

- How do they exchange keys?
- Which algorithm for key exchange?
- Which algorithm for encrypting the actual message?

---

## Scenario C — Verifying downloaded software

You want users to trust that the `.exe` they downloaded wasn’t changed.

Questions:

- What cryptographic mechanism do you need?
- Which algorithms can be used?

---

## Scenario D — API request authentication

Your API receives requests like this:

```
GET /balance
Authorization: <signature>
```

Questions:

- Should you use encryption?
- Or hashing?
- Or HMAC?
- What does the signature prove?

---

## Scenario E — Password storage for a website

Ask:

- SHA-256 acceptable for password storage?
- What should you do instead?
