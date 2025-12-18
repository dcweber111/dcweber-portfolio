dcweber INFO 1031 12-21-25
Wireframe: of portfolio and eCommerce Shopping Cart
1) Sticky Navigation Bar (top)
┌───────────────────────────────────────────────────────────────────────────┐
│  [INFO1031 logo/name]     [About] [Projects] [Skills] [Contact]   │icons│ │
│                                                             Git In Tw  ☼/☾│
└───────────────────────────────────────────────────────────────────────────┘
•	Left: site name/logo
•	Center/right: section links (hidden on mobile)
•	Right: social icons (GitHub/LinkedIn/Twitter) + theme toggle
 
2) Hero Section (intro)
┌───────────────────────────────────────────────────────────────────────────┐
│  (Decorative gradient background layer behind content)                    │
│                                                                           │
│  ┌──────────────────────────────┐    ┌───────────────────────────────┐   │
│  │  Headline (your name/role)    │    │   Profile photo (circular /   │   │
│  │  Short intro paragraph         │    │   framed image)               │   │
│  │  Primary CTA button(s)         │    └───────────────────────────────┘   │
│  │  Secondary CTA / links         │                                       │
│  └──────────────────────────────┘                                       │
│                                                                           │
└───────────────────────────────────────────────────────────────────────────┘
•	Two-column layout: intro text + profile image
•	Decorative gradient element behind
 
3) About Section
┌───────────────────────────────────────────────────────────────────────────┐
│                         ABOUT (section title)                             │
│                         ───── (accent divider)                            │
│  ┌─────────────────────────────────────────────────────────────────────┐  │
│  │ Background / bio text (paragraphs)                                   │  │
│  │ Possibly bullet highlights (experience, focus areas, etc.)            │  │
│  └─────────────────────────────────────────────────────────────────────┘  │
│                          (decorative circle shape)                         │
└───────────────────────────────────────────────────────────────────────────┘
 
4) Projects Section (cards grid)
┌───────────────────────────────────────────────────────────────────────────┐
│                        PROJECTS (section title)                            │
│                         ───── (accent divider)                             │
│  ┌───────────────┐   ┌───────────────┐   ┌───────────────┐                │
│  │ [Image]        │   │ [Image]        │   │ [Image]        │                │
│  │ Title          │   │ Title          │   │ Title          │                │
│  │ Description    │   │ Description    │   │ Description    │                │
│  │ [Tech tags]    │   │ [Tech tags]    │   │ [Tech tags]    │                │
│  │ [GitHub][Demo] │   │ [GitHub][Demo] │   │ [GitHub][Demo] │                │
│  └───────────────┘   └───────────────┘   └───────────────┘                │
└───────────────────────────────────────────────────────────────────────────┘
•	3-up grid on desktop
•	Each card has: image → title → description → tech tags → action buttons
 
5) Skills Section (progress bars + tags)
┌───────────────────────────────────────────────────────────────────────────┐
│                         SKILLS (section title)                             │
│                         ───── (accent divider)                             │
│   ┌─────────────────────────────┐   ┌─────────────────────────────┐        │
│   │ Frontend Skills             │   │ Backend Skills              │        │
│   │ React/Next.js   95% [====]  │   │ Node/Express    85% [====]  │        │
│   │ TypeScript      90% [====]  │   │ DB Design       80% [=== ]  │        │
│   │ UI/UX           85% [=== ]  │   │ GraphQL         75% [==  ]  │        │
│   └─────────────────────────────┘   └─────────────────────────────┘        │
│                                                                           │
│  Other Technologies: [Docker] [AWS] [CI/CD] [Jest] [Git] [Redux] ...      │
└───────────────────────────────────────────────────────────────────────────┘
•	Two columns: frontend + backend skill meters
•	Below: “pill” tags for other technologies
 
6) Contact Section (form)
┌───────────────────────────────────────────────────────────────────────────┐
│                        CONTACT (section title)                             │
│                         ───── (accent divider)                             │
│  ┌─────────────────────────────────────────────────────────────────────┐  │
│  │ [Name field]                                                         │  │
│  │ [Email field]                                                        │  │
│  │ [Message field (multi-line)]                                         │  │
│  │                       [Send button]                                  │  │
│  └─────────────────────────────────────────────────────────────────────┘  │
│  (Optional: email icon / social links repeated)                            │
└───────────────────────────────────────────────────────────────────────────┘
 
7) Footer
┌───────────────────────────────────────────────────────────────────────────┐
│  © Year Your Name — All rights reserved                                   │
└───────────────────────────────────────────────────────────────────────────┘
 
Wireframe: Mobile layout (xs)
Key changes implied by your code:
•	Nav links hide (About/Projects/Skills/Contact won’t show in the top bar)
•	Top bar becomes:
┌──────────────────────────────────────┐
│ [INFO1031]          [icons]    ☼/☾    │
└──────────────────────────────────────┘
•	Hero becomes stacked:
[Profile photo]
[Headline + intro]
[Buttons]
•	Projects become 1 card per row
•	Skills become stacked sections instead of 2 columns
 
If you paste a little more of your file (right after the Hero section continues), I can map the wireframe exactly to your section IDs and components (like id="about", id="projects", etc.) and match the actual layout hierarchy line-for-line.
Desktop Wireframe (md+)
Global Page Frame
┌──────────────────────────────────────────────────────────────────────────────┐
│  PAGE BACKGROUND (subtle gradient)                                           │
│                                                                              │
│  [1] STICKY NAV BAR                                                          │
│  [2] HERO                                                                    │
│  [3] ABOUT                                                                   │
│  [4] PROJECTS                                                                │
│  [5] SKILLS                                                                  │
│  [6] CONTACT                                                                 │
│  [7] FOOTER                                                                  │
└──────────────────────────────────────────────────────────────────────────────┘
 
1) Sticky Navigation Bar (Top)
┌──────────────────────────────────────────────────────────────────────────────┐
│  ┌────────────────────────────────────────────────────────────────────────┐  │
│  │ [INFO1031 / Logo]      [About] [Projects] [Skills] [Contact]   [Icons] │  │
│  │                                                         [Git][In][Tw] │  │
│  │                                                               [☼/☾]   │  │
│  └────────────────────────────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────────────────────────────┘
Zones
•	Left: Brand / identity
•	Middle: Section links (scroll targets)
•	Right: Social icons + theme toggle
 
2) Hero Section (Intro)
┌──────────────────────────────────────────────────────────────────────────────┐
│  HERO SECTION (large padding, decorative gradient behind)                    │
│                                                                              │
│  [Background Layer]                                                          │
│   └─ angled gradient shape (very subtle opacity)                             │
│                                                                              │
│  [Content Layer] (centered container, two-column grid)                       │
│                                                                              │
│  ┌───────────────────────────────────┐     ┌──────────────────────────────┐ │
│  │  H1: Your Name / Role              │     │   Profile Image              │ │
│  │  Subtitle: short positioning line  │     │   (circle/frame + shadow)   │ │
│  │  Paragraph: 2–4 line intro         │     └──────────────────────────────┘ │
│  │                                   │                                       │
│  │  [Primary CTA Button]  [Secondary]│                                       │
│  │  (optional micro-links / badges)  │                                       │
│  └───────────────────────────────────┘                                       │
└──────────────────────────────────────────────────────────────────────────────┘
Purpose
•	Immediately communicates: who you are + what you do + where to click next
 
3) About Section
┌──────────────────────────────────────────────────────────────────────────────┐
│  ABOUT                                                                       │
│  ┌────────────────────────────────────────────────────────────────────────┐  │
│  │               ABOUT (title centered)                                     │  │
│  │               ───── (accent divider)                                     │  │
│  │                                                                          │  │
│  │  ┌────────────────────────────────────────────────────────────────────┐  │  │
│  │  │  Bio paragraphs (background, goals, what you build)                 │  │  │
│  │  │                                                                      │  │  │
│  │  │  Optional bullets:                                                   │  │  │
│  │  │   • Focus area 1                                                     │  │  │
│  │  │   • Focus area 2                                                     │  │  │
│  │  │   • Focus area 3                                                     │  │  │
│  │  └────────────────────────────────────────────────────────────────────┘  │  │
│  │                                                                          │  │
│  │                 (decorative circle shape behind corner)                  │  │
│  └────────────────────────────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────────────────────────────┘
 
4) Projects Section (Cards Grid)
┌──────────────────────────────────────────────────────────────────────────────┐
│  PROJECTS                                                                    │
│  ┌────────────────────────────────────────────────────────────────────────┐  │
│  │               PROJECTS (title centered)                                  │  │
│  │               ───── (accent divider)                                     │  │
│  │                                                                          │  │
│  │  ┌───────────────┐  ┌───────────────┐  ┌───────────────┐                │  │
│  │  │ [Image Header] │  │ [Image Header] │  │ [Image Header] │               │  │
│  │  │ Title          │  │ Title          │  │ Title          │               │  │
│  │  │ Description    │  │ Description    │  │ Description    │               │  │
│  │  │ [Tag][Tag][..] │  │ [Tag][Tag][..] │  │ [Tag][Tag][..] │               │  │
│  │  │ [GitHub][Demo] │  │ [GitHub][Demo] │  │ [GitHub][Demo] │               │  │
│  │  └───────────────┘  └───────────────┘  └───────────────┘                │  │
│  └────────────────────────────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────────────────────────────┘
Card anatomy
•	Top: image/thumbnail
•	Middle: title + description
•	Lower: tags
•	Bottom: action buttons
 
5) Skills Section (Meters + Tags)
┌──────────────────────────────────────────────────────────────────────────────┐
│  SKILLS                                                                      │
│  ┌────────────────────────────────────────────────────────────────────────┐  │
│  │                 SKILLS (title centered)                                  │  │
│  │                 ───── (accent divider)                                   │  │
│  │                                                                          │  │
│  │  ┌─────────────────────────────┐     ┌─────────────────────────────┐     │  │
│  │  │ Frontend Skills             │     │ Backend Skills              │     │  │
│  │  │ React/Next.js   95% [████]  │     │ Node/Express    85% [███ ]  │     │  │
│  │  │ TypeScript      90% [████]  │     │ DB Design       80% [███ ]  │     │  │
│  │  │ UI/UX           85% [███ ]  │     │ GraphQL         75% [██  ]  │     │  │
│  │  └─────────────────────────────┘     └─────────────────────────────┘     │  │
│  │                                                                          │  │
│  │  Other Technologies (pill tags row/wrap):                                │  │
│  │  [Docker] [AWS] [CI/CD] [Jest] [Git] [Redux] [Firebase] ...              │  │
│  └────────────────────────────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────────────────────────────┘
 
6) Contact Section (Form)
┌──────────────────────────────────────────────────────────────────────────────┐
│  CONTACT                                                                     │
│  ┌────────────────────────────────────────────────────────────────────────┐  │
│  │                CONTACT (title centered)                                  │  │
│  │                ───── (accent divider)                                    │  │
│  │                                                                          │  │
│  │  ┌────────────────────────────────────────────────────────────────────┐  │  │
│  │  │  [ Name _________________________________ ]                          │  │  │
│  │  │  [ Email ________________________________ ]                          │  │  │
│  │  │  [ Message ______________________________ ]                          │  │  │
│  │  │  [______________________________________ ]                          │  │  │
│  │  │                                                                          │  │
│  │  │                      [ Send Message Button ]                          │  │  │
│  │  └────────────────────────────────────────────────────────────────────┘  │  │
│  │                                                                          │  │
│  │  Optional: repeat social icons / email link                               │  │
│  └────────────────────────────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────────────────────────────┘
 
7) Footer
┌──────────────────────────────────────────────────────────────────────────────┐
│  © 2025 Your Name — All rights reserved                                      │
└──────────────────────────────────────────────────────────────────────────────┘
 
Mobile Wireframe (xs)
Navigation (links hidden)
┌──────────────────────────────────────────────┐
│ [INFO1031]               [Git][In][Tw] [☼/☾] │
└──────────────────────────────────────────────┘
Hero (stacked)
┌──────────────────────────────────────────────┐
│ [Profile Image]                              │
│ H1: Name / Role                              │
│ Short intro paragraph                         │
│ [Primary CTA]                                │
│ [Secondary CTA]                              │
└──────────────────────────────────────────────┘
Projects (single column cards)
┌──────────────────────────────────────────────┐
│ [Card 1]                                     │
│ [Card 2]                                     │
│ [Card 3]                                     │
└──────────────────────────────────────────────┘
Skills (stacked)
┌──────────────────────────────────────────────┐
│ Frontend Skills (meters)                      │
│ Backend Skills (meters)                       │
│ Tech tags (wrap)                              │
└──────────────────────────────────────────────┘



 SHOPPING CART
Main actions
•	Review items in cart
•	Enter or confirm shipping information
•	Select payment method
•	Review order details
•	Submit payment
Expected outcome
•	Order is successfully placed
•	User receives confirmation and order summary


Frame 1: Shopping Cart Review
Purpose
•	Let users confirm what they are buying before checkout.
┌──────────────────────────────────────────────┐
│ Header                                       │
│ [Logo]                   [Cart Icon]        │
├──────────────────────────────────────────────┤
│ CART                                         │
│                                              │
│ ┌──────────────────────────────────────────┐ │
│ │ Item Thumbnail  Item Name                │ │
│ │ Qty: [-] 1 [+]   Price                   │ │
│ │ [Remove]                                 │ │
│ └──────────────────────────────────────────┘ │
│                                              │
│ ┌──────────────────────────────────────────┐ │
│ │ Item Thumbnail  Item Name                │ │
│ │ Qty: [-] 2 [+]   Price                   │ │
│ │ [Remove]                                 │ │
│ └──────────────────────────────────────────┘ │
│                                              │
│ Subtotal: $XX.XX                             │
│ Estimated Tax: $X.XX                         │
│ Total: $XX.XX                               │
│                                              │
│ [Continue Shopping]   [Proceed to Checkout] │
└──────────────────────────────────────────────┘
Interactive elements
•	Quantity controls
•	Remove item
•	Proceed to Checkout (primary action)
Flow
•	➜ Clicking Proceed to Checkout moves to Shipping Information
 
Frame 2: Shipping Information
Purpose
•	Collect delivery details.
┌──────────────────────────────────────────────┐
│ Header                                       │
│ Checkout Progress: Cart → Shipping → Payment │
├──────────────────────────────────────────────┤
│ SHIPPING INFORMATION                          │
│                                              │
│ [Full Name ____________________________]     │
│ [Street Address _______________________ ]    │
│ [City __________ ] [State ____ ] [ZIP ____ ] │
│ [Country _____________________________ ]     │
│ [Phone Number ________________________ ]     │
│                                              │
│ ☐ Save address for future purchases          │
│                                              │
│ [Back to Cart]        [Continue to Payment]  │
└──────────────────────────────────────────────┘
Interactive elements
•	Text input fields
•	Checkbox
•	Continue to Payment (primary action)
Flow
•	➜ Continue to Payment
•	← Back to Cart
 
Frame 3: Payment Method
Purpose
•	Choose and enter payment details securely.
┌──────────────────────────────────────────────┐
│ Header                                       │
│ Checkout Progress: Cart → Shipping → Payment │
├──────────────────────────────────────────────┤
│ PAYMENT METHOD                                │
│                                              │
│ ⦿ Credit / Debit Card                        │
│ ⦾ PayPal                                    │
│ ⦾ Apple Pay / Google Pay                    │
│                                              │
│ [Card Number __________________________]     │
│ [Name on Card __________________________]    │
│ [Expiration __ / __ ]   [CVV ___ ]           │
│                                              │
│ Billing Address                              │
│ ⦿ Same as shipping                           │
│ ⦾ Use different billing address              │
│                                              │
│ [Back to Shipping]   [Review Order]          │
└──────────────────────────────────────────────┘
Interactive elements
•	Radio buttons
•	Card fields
•	Review Order button
Flow
•	➜ Review Order
•	← Back to Shipping
 
Frame 4: Order Review
Purpose
•	Final confirmation before purchase.
┌──────────────────────────────────────────────┐
│ Header                                       │
│ Checkout Progress: Cart → Shipping → Payment │
├──────────────────────────────────────────────┤
│ REVIEW YOUR ORDER                             │
│                                              │
│ Items Summary                                │
│ - Item Name x1  $XX.XX                       │
│ - Item Name x2  $XX.XX                       │
│                                              │
│ Shipping Address                             │
│ John Doe                                     │
│ 123 Main St, City, State ZIP                 │
│                                              │
│ Payment Method                               │
│ Credit Card ending in 1234                   │
│                                              │
│ Subtotal: $XX.XX                             │
│ Tax: $X.XX                                  │
│ Shipping: $X.XX                              │
│ Total: $XX.XX                               │
│                                              │
│ [Edit Cart]  [Edit Payment]  [Place Order]  │
└──────────────────────────────────────────────┘
Interactive elements
•	Edit links
•	Place Order (primary CTA)
Flow
•	➜ Place Order
 
Frame 5: Order Confirmation
Purpose
•	Reassure the user and confirm success.
┌──────────────────────────────────────────────┐
│ Header                                       │
├──────────────────────────────────────────────┤
│ ✅ ORDER CONFIRMED                            │
│                                              │
│ Thank you for your purchase!                 │
│                                              │
│ Order Number: #123456                        │
│ Confirmation Email Sent To: user@email.com  │
│                                              │
│ Estimated Delivery: June 10–12               │
│                                              │
│ [View Order Details]                         │
│ [Continue Shopping]                          │
└──────────────────────────────────────────────┘
Outcome
•	User feels confident purchase was successful
•	Clear next steps available
 
User Flow Overview
Cart Review
     ↓
Shipping Information
     ↓
Payment Method
     ↓
Order Review
     ↓
Order Confirmation
Arrows in Figma Prototype Mode should connect:
•	Buttons → next screen
•	Back links → previous screen

<img width="468" height="636" alt="image" src="https://github.com/user-attachments/assets/727c26e7-ac45-4a1e-a05e-cf7118979ad8" />
