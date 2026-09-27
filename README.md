# Password-hash.github.io

A tiny educational demo that shows how password authentication *should* work.

## What it demonstrates

1. User types a password
2. The password is immediately turned into a **SHA-256 hash**
3. That hash is compared to a **pre-stored hash** of the correct password
4. The original password is **never stored**

## How to run

Just open `index.html` in any modern browser.  
No server or install needed.

## Correct credentials

- Username: `admin` (fixed)
- Password: `secret123`

## Notes

- This uses the browser’s built-in Web Crypto API.
- In production you would also use a unique **salt** and a slow hashing algorithm (bcrypt, scrypt, or Argon2).
- Never roll your own crypto in real applications.
