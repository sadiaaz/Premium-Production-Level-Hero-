📱 Premium Hero Section with Cinematic Animation

A modern, high-end hero section built with pure HTML, CSS, and JavaScript featuring:

Smooth page fade redirect

Swiper-compatible structure

Samsung-style cinematic entrance animation

Glass morphism hover overlay

Cursor-based ripple click effect

🚀 Features
1️⃣ Smooth Page Transition

The page fades out smoothly before redirecting to another URL using a CSS opacity transition.

2️⃣ Cinematic Text Animation

Hero content fades in and slides upward on load for a premium product-launch feel.

3️⃣ Glass Morphism Overlay

Uses backdrop-filter: blur() with semi-transparent dark overlay for a modern UI effect.

4️⃣ Ripple Click Effect

Clicking anywhere on the hero creates a ripple animation from the cursor position.

5️⃣ Swiper Compatible

The structure supports integration inside Swiper.js sliders.

📂 Project Structure
index.html


All CSS and JavaScript are embedded inside the HTML file for simplicity.

🧩 How It Works
Smooth Redirect Logic
function smoothRedirect(event, url) {
    event.preventDefault();
    document.body.classList.add("fade-out");

    setTimeout(() => {
        window.location.href = url;
    }, 600);
}


The fade-out class reduces body opacity before navigating.

Ripple Effect Logic

When the button is clicked:

A <span> is dynamically created.

Positioned at cursor coordinates.

Scaled using CSS animation.

Automatically removed after animation completes.

🔌 Swiper Integration

To use inside Swiper:

<div class="swiper-wrapper">
   <div class="swiper-slide hero-slide">
      <!-- hero content -->
   </div>
</div>


No structural changes required.

🎨 Customization
Change Background Image

Modify this inside CSS:

background: url("your-image.jpg") center/cover no-repeat;

Change Redirect URL
onclick="smoothRedirect(event, 'https://your-link.com')"

🌐 Browser Support

Chrome ✅

Edge ✅

Firefox ✅

Safari ⚠ (backdrop-filter support required)

⚡ Performance Notes

No external libraries required

Lightweight

Fully responsive

Mobile compatible

🛠 Future Enhancements (Optional)

Parallax mouse tracking

3D tilt interaction

Scroll-triggered animations

Video background support

Apple-style dynamic lighting effect

📄 License

Free to use and modify for personal and commercial projects.
