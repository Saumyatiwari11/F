# LitShelf – Original Multi-Seller Book Marketplace

**LitShelf** is an original web app for buying and selling **books only**.  
It is **not** affiliated with or copied from any other marketplace brand.

## Identity
- Name: LitShelf  
- Theme: warm cream + soft sage (bookish, original)  
- Focus: independent booksellers ↔ customers  

## Roles
| Role | Can do |
|------|--------|
| **Customer** | Browse, search/filter, cart, checkout (COD / demo online), track orders |
| **Seller** | List books, manage stock, process orders (Confirmed → Shipped → Delivered) |
| **Admin** | Approve sellers, view all books & orders |

## Practical flow
1. **Admin** (optional): approve new sellers under Sellers.  
2. **Seller**: My Listings → + List a Book (title, price, stock, condition…).  
3. **Customer**: Browse → Add to Cart → Checkout. Stock decreases; oversell blocked.  
4. **Seller**: Orders → update status. Customer sees the same status.  

Catalog starts **empty** until sellers add books.

## Demo accounts
| Role | Email | Password |
|------|-------|----------|
| Admin | admin@litshelf.com | admin123 |
| Seller | seller@litshelf.com | seller123 |
| Seller 2 | vikram@litshelf.com | seller123 |
| Customer | customer@litshelf.com | cust123 |

New sellers can Sign Up; they need admin approval before listing.

## Deploy on Vercel
1. Unzip this folder.  
2. Go to https://vercel.com/new  
3. Drag the `litshelf` folder → Deploy.  

Live URL example: `https://litshelf-xxxx.vercel.app`

## Local preview
Open `index.html` via a static server, or deploy as above. API is at `/api`.

## Tech
- Static HTML/CSS/JS frontend  
- Vercel Serverless Function (`/api`)  
- In-memory + seed JSON (fine for demo; swap to MongoDB later for production)

## Legal
- No third-party brand names, logos, or UI clones in this project.  
- Book cover URLs are optional user-provided or free placeholders only.

## Navigation (updated)
- Demo account list removed from the login screen (frontend only).
- In-app pages use browser history (`#/dashboard`, `#/catalog`, etc.).
- Phone swipe-back / browser Back moves between app screens only.
- Logged-in users are not sent back to the login page on Back.
- Logout clears session and resets history to the auth screen.
