# DMI Portfolio Website (Static HTML/CSS)

This repository contains a clean, professional-looking **static portfolio website** used in **DevOps Micro Internship (DMI)** Week 1 to practice:
- Linux basics
- Nginx hosting
- Deployment proof / ownership
- Production-style checks

✅ Students deploy this website on an Ubuntu VM using Nginx and keep it live for 24 hours.

---

## Who is this for?
- DMI students (beginner → intermediate)
- Anyone learning how to host a static site with Nginx on Linux

---

## What you will build
A portfolio-style website hosted on:
- **Ubuntu VM**
- **Nginx**
- Accessible via: `http://44.222.176.128/`

---

## Mandatory Ownership Proof (DMI Rule)
Before you deploy, you MUST edit the footer and add your details:

Original:

```html
<p>Crafted with <span>cloud</span> excellence by Pravin Mishra</p>
```

Add this line (example):

```html
<p>Pravin Mishra Portfolio v1.0 — Deployed on <span id="deployDate">05 Feb 2026</span> — By Varun Gopal<p>
```
JavaScript:
```html
<!-- Bottom -->
      <div class="footer-bottom">
        <p>© <span id="year"></span> <span style="font-size: 20px;">  Pravin Mishra</span>. All rights reserved.</p>
         <p>Crafted with <span>cloud</span> excellence by Pravin Mishra</p>
         <p>Pravin Mishra Portfolio v1.0 — Deployed on <span id="deployDate">05 Feb 2026</span> — By Varun Gopal<p>
       </div>

       <script>
         const d = new Date();
         const formattedDate = d.toISOString().split('T')[0];
         document.getElementById("deployDate").textContent = formattedDate;
       </script>
     </div>
   </footer>
```
✅ This proof must be visible in your browser screenshot submission.