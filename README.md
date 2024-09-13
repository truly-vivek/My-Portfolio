# My-Portfolio

Welcome to my personal portfolio website showcasing my skills, experience, and projects. This portfolio is a reflection of my journey as a developer, and you can explore my work, achievements, and connect with me!

## Live Preview
Check out my portfolio live at [Vivek's Portfolio](https://vivek76.vercel.app/).

## Features
- **Responsive Design:** Fully responsive across all devices.
- **Dynamic Typing Text:** Engaging introduction with dynamic typing effect.
- **Interactive UI:** Smooth transitions, hover effects, and engaging animations.
- **Project Showcase:** Detailed descriptions and links to GitHub repositories for my key projects.
- **AI Chat Assistant:** A simple AI chatbot integrated into the site to assist visitors.
- **EmailJS Contact Form:** A serverless email form that sends messages directly from the website.
- **Social Links:** Direct links to my GitHub, LinkedIn, and other platforms.

## Sections
- **Home:** Introduction and social links.
- **About Me:** A brief bio and my professional background.
- **Skills:** A showcase of my technical skills and tools I work with.
- **Education:** My academic qualifications.
- **Work & Projects:** Featured projects with live demos and source code links.
- **Experience:** Professional experience and internships.
- **Contact:** A form for direct communication and links to my social profiles.

## AI Chat Integration

This portfolio features an AI chat assistant that helps visitors navigate the website or answer basic queries.

EmailJS Contact Form
--------------------

The contact form in this portfolio allows users to send me messages directly through the website. The form is powered by EmailJS, enabling serverless email functionality.

### How it Works

-   **Technology:** EmailJS enables sending emails directly from the client-side.
-   **Form Fields:** Name, email, phone number, and message.
-   **Integration:** JavaScript code integrates the form with EmailJS, which handles the email delivery.

### Setup Instructions

1.  Create an account on [EmailJS](https://www.emailjs.com/).

2.  Create a new service and get the Service ID, Template ID, and User ID.

3.  Update the form code in the `index.html` as follows:
  ```bash
   <form id="contact-form">
  <input type="text" name="name" placeholder="Name" required />
  <input type="email" name="email" placeholder="Email" required />
  <input type="text" name="phone" placeholder="Phone" />
  <textarea name="message" placeholder="Message" required></textarea>
  <button type="submit">Send Message</button>
</form>

<script type="text/javascript">
  (function () {
    emailjs.init('YOUR_USER_ID');
  })();

  document.getElementById('contact-form').addEventListener('submit', function (event) {
    event.preventDefault();
    emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', this)
      .then(function () {
        alert('Message sent successfully!');
      }, function (error) {
        alert('Failed to send message, please try again.');
      });
  });
</script>
```
Technologies Used
-----------------

-   **Frontend:** HTML5, CSS3, JavaScript
-   **Icons & Fonts:** Font Awesome
-   **Hosting:** Vercel
-   **Version Control:** GitHub
-   **Animations:** Typed.js, ScrollReveal.js, Vanilla Tilt.js
-   **Backend:** Firebase (for analytics)

Installation
------------

To set up the portfolio locally, follow these steps:

### Prerequisites

Ensure you have the following installed on your machine:

-   A web browser (Google Chrome, Firefox, etc.)
-   [Git](https://git-scm.com/)
### Step-by-Step Instructions

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/truly-vivek/My-Portfolio.git
    ```
2. **Navigate to the Project Directory:**

    ```bash
    cd My-Portfolio
    ```
3. **Open `index.html` in Browser:**

If no advanced setup is needed, simply open the `index.html` file in your browser to view the portfolio.
  ```bash
   open index.html
```
Or, manually navigate to the file and double-click index.html to open it in your preferred web browser.
## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

---

## Copyright

&copy; 2024 Vivek Reddy Kesavarapu. All rights reserved.

Permission is granted to use this resume template for personal use, but it may not be reproduced, distributed, or used for any commercial purposes without explicit permission from the author.
