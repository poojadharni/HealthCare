<template>
<section class="mt-8 relative w-full bg-cover h-72" style="background-image: url('/images/contactUs.png'); background-position: center 25%;">
    <!-- White transparent overlay -->
    <div class="absolute inset-0 bg-white bg-opacity-50"></div>

    <!-- Content above overlay -->
    <div class="relative z-10 flex items-center justify-center h-full">
        <h1 class="text-7xl font-bold text-blue-900">Our Contacts</h1>
    </div>
</section>
<section class="mt-4 h-[400px] max-w-5xl mx-auto">
    <iframe class="w-full h-full rounded-lg shadow-md" src="https://www.google.com/maps?q=No.1376,+2nd+floor,+13th+Cross,+Sarakki+Main+Rd,+1st+Phase,+J.+P.+Nagar,+Bengaluru,+Karnataka+560078&output=embed" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
    </iframe>
</section>
<section class="max-w-5xl mx-auto px-6 py-12 grid lg:grid-cols-2 gap-6">
    <!-- Contact Form -->
    <div class="w-full max-w-md">
        <!-- Headings -->
        <div class="mb-6">
            <h3 class="text-sm font-bold text-blue-600 tracking-wide">GET IN TOUCH</h3>
            <h2 class="text-2xl font-bold text-[#1F2B6C]">Contact</h2>
        </div>

        <!-- Form -->
        <div class="bg-[#1F2B6C] text-white">
            <form class="border border-blue-900 ">
                <!-- Grid Inputs with Lines -->
                <div class="grid grid-cols-2 ">
                    <input type="text" placeholder="Name" class="bg-transparent px-3 py-2 placeholder-white border-b focus:outline-none" />

                    <input type="email" placeholder="Email" class="bg-transparent px-3 py-2 placeholder-white border-b focus:outline-none" />
                </div>
                <input type="subject" placeholder="Subject" class="w-full bg-transparent px-3 py-2 placeholder-white border-b focus:outline-none" />

                <!-- Message Box -->
                <textarea placeholder="Message" rows="4" class="w-full bg-transparent placeholder-white px-3 py-2 outline-none border-none focus:outline-none focus:ring-0"></textarea>

                <!-- Submit Button -->
                <button type="submit" class="w-full bg-[#BFD2F8] text-[#1F2B6C] font-bold py-2 hover:bg-blue-400 transition-colors">
                    SUBMIT
                </button>
            </form>
        </div>
    </div>

    <!-- Contact Info Cards -->
    <div class="grid grid-cols-2 gap-4">
        <div class="bg-[#BFD2F8] p-4 rounded-lg border border-blue-300 flex flex-col items-start">
            <i class="fas fa-phone-alt text-blue-600 text-3xl mb-4"></i>
            <span class="text-lg font-bold mb-2">EMERGENCY</span>
            <p class="text-sm">(237) 681-812-255</p>
            <p class="text-sm">(237) 666-331-894</p>
        </div>
        <div class="bg-[#1F2B6C] text-white p-4 rounded-lg border border-blue-300 flex flex-col items-start">
            <i class="fas fa-map-marker-alt text-white text-3xl mb-4"></i>
            <span class="text-lg font-bold mb-2">LOCATION</span>
            <p class="text-sm">0123 Some place</p>
            <p class="text-sm">9876 Some country</p>
        </div>
        <div class="bg-[#BFD2F8] p-4 rounded-lg border border-blue-300 flex flex-col items-start">
            <i class="fas fa-envelope text-blue-600 text-3xl mb-4"></i>
            <span class="text-lg font-bold mb-2">EMAIL</span>
            <p class="text-sm">fildineeesoe@gmail.com</p>
            <p class="text-sm">myebstudios@gmail.com</p>
        </div>
        <div class="bg-[#BFD2F8] p-4 rounded-lg border border-blue-300 flex flex-col items-start">
            <i class="fas fa-clock text-blue-600 text-3xl mb-4"></i>
            <span class="text-lg font-bold mb-2">WORKING HOURS</span>
            <p class="text-sm">Mon-Sat 09:00-20:00</p>
            <p class="text-sm">Sunday Emergency only</p>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: "ContactForm",
  data() {
    return {
      form: {
        name: "",
        email: "",
        subject: "",
        message: ""
      }
    }
  },
  methods: {
    handleSubmit() {
      alert(`Form submitted: ${JSON.stringify(this.form)}`)
    }
  }
}
</script>

