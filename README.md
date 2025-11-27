# 👕 Custom T-Shirt Designer & Print Order Tool

A full-stack web application that allows users to design custom t-shirts using a visual canvas and immediately send order details to print sellers.

![Project Screenshot](https://via.placeholder.com/800x400?text=Upload+Your+Screenshot+Here)
*(Tip: Replace the link above with a screenshot of your actual tool once uploaded!)*

## 🚀 Features

* **Interactive Design Canvas:** Built with HTML5 Canvas, allowing users to drag, drop, resize, and colorize design elements.
* **Real-time Preview:** Users see exactly how the print will look on the t-shirt.
* **Send Ordering:** Integrates with **Nodemailer** to send the final design file and order details directly to the print seller's email.
* **Responsive UI:** Fully responsive design built with **Tailwind CSS**.
* **Server-Side Rendering:** Optimized performance using **Next.js**.

## 🛠️ Tech Stack

* **Framework:** [Next.js](https://nextjs.org/)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **Graphics:** HTML5 Canvas API
* **Email Service:** [Nodemailer](https://nodemailer.com/)

## 📦 Getting Started

Follow these steps to set up the project locally on your machine.

### Prerequisites

* Node.js (v14 or higher)
* npm or yarn

### Installation

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/tshirt-designer-tool.git](https://github.com/YOUR_USERNAME/tshirt-designer-tool.git)
    cd tshirt-designer-tool
    ```

2.  **Install dependencies**
    ```bash
    npm install
    # or
    yarn install
    ```

3.  **Set up Environment Variables**
    Create a `.env.local` file in the root directory. You will need this for the email functionality to work.
    
    ```env
    # .env.local
    EMAIL_USER=your_email@gmail.com
    EMAIL_PASS=your_app_password
    RECEIVER_EMAIL=print_seller@example.com
    ```
    *> **Note:** If using Gmail, make sure to generate an "App Password" rather than using your main login password.*

4.  **Run the development server**
    ```bash
    npm run dev
    ```

5.  Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## 📧 How the Email Logic Works

When a user clicks "Send to Print":
1.  The Canvas converts the design into a base64 image string or Blob.
2.  Next.js API routes receive the image and user details.
3.  **Nodemailer** constructs an email with the design attached and sends it to the configured print shop address.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

**Developed by [thimiraSH]**
