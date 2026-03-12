# Donation Website

A responsive donation website built for **The Sparks Foundation** with integrated Razorpay payment gateway. Users can browse the landing page, make donations via a secure payment flow, and receive confirmation upon successful payment.

## Live Demo

> _[Add your Netlify URL here after deployment]_

## Features

- **Responsive Design** — Fully optimized for desktop and mobile devices with hamburger navigation on smaller screens
- **Payment Gateway Integration** — Razorpay payment button for secure, real-time donations
- **Smooth Animations** — Page transitions and element animations powered by GSAP (GreenSock)
- **Contact Form** — Styled with Tailwind CSS for a clean, modern look
- **Post-Payment Flow** — Thank you page with success confirmation and auto-redirect

## Pages

| Page | Description |
|------|-------------|
| **Home** | Hero landing page with a call-to-action to donate |
| **Donate** | Donation form with Razorpay payment integration |
| **Contact** | Contact form with name, email, and message fields |
| **Thank You** | Payment success confirmation with auto-redirect |

## Tech Stack

- **HTML5** — Semantic markup
- **CSS3** — Custom styles with responsive media queries
- **JavaScript** — DOM manipulation and event handling
- **GSAP (GreenSock)** — Scroll and load animations
- **Tailwind CSS** — Utility-first styling (Contact page)
- **Razorpay** — Payment gateway integration

## Project Structure

```
Donation-Website/
└── public/
    ├── index.html              # Home page
    ├── Donation.html           # Donation page with Razorpay
    ├── contact.html            # Contact form
    ├── thankyou.html           # Payment success page
    ├── 404.html                # Custom 404 page
    ├── css/
    │   ├── style.css           # Global styles & responsive layout
    │   ├── donation.css        # Donation page styles
    │   └── thankyou.css        # Thank you page styles
    ├── js/
    │   ├── homepage-animations.js    # Home page GSAP animations
    │   ├── donation-animations.js    # Donation page animations
    │   ├── ham-animation.js          # Hamburger menu toggle
    │   └── thankyou.js               # Success page animation & redirect
    └── material/
        ├── bg-cover.jpg        # Home page background
        ├── bg-cover1.jpg       # Alternate background
        ├── thankyou.jpg        # Thank you page background
        └── success.gif         # Success animation
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (for local dev server)

### Run Locally

```bash
cd Donation-Website/public
npx serve .
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Alternative (Python)

```bash
cd Donation-Website/public
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) in your browser.

## Configuration

To use your own Razorpay account, replace the payment button ID in `Donation.html`:

```html
<script src="https://checkout.razorpay.com/v1/payment-button.js"
    data-payment_button_id="YOUR_PAYMENT_BUTTON_ID" async>
</script>
```

You can generate a payment button ID from the [Razorpay Dashboard](https://dashboard.razorpay.com/app/payment-button).