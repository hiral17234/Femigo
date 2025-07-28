# femigo-women-navigation-app
# 𝐅𝐞𝐦𝐢𝐠𝐨 — 𝐘𝐨𝐮𝐫 𝐏𝐞𝐫𝐬𝐨𝐧𝐚𝐥 𝐒𝐚𝐟𝐞𝐭𝐲 𝐚𝐧𝐝 𝐂𝐨𝐧𝐧𝐞𝐜𝐭𝐢𝐯𝐢𝐭𝐲 𝐂𝐨𝐦𝐩𝐚𝐧𝐢𝐨𝐧
It is a smart, privacy-focused, and empowering mobile application designed to enhance women's safety and well-being. Built with a vision to merge technology with trust, it offers real-time location tracking, emergency check, live status updates &amp; community safety checks-all in one place.

## ✨ Features

🔴 SOS Emergency Alerts - Instantly notify trusted contacts with your live location and custom message.

📍 Live Location Tracking - Real-time location sharing with selected friends or guardians.

💬 Safety ChatBot with AI - A friendly, 24x7 AI assistant to guide users in unsafe situations or emergencies.

🛡️ One-Tap Safety Check (SafeSage) - Quick self-checks + custom actions (like send location, trigger alert, or connect with help line).

📌 Nearby Safe Places (Future Integration) - Discover nearby police stations, hospitals, or women-only safe zones.

👣 Geo-Gesture & Voice Activation (Upcoming) - Activate emergency features via voice commands or motion gestures like shaking the phone.

## 🚀 Tech Stack

Frontend: Flutter / React Native (customizable)

Backend: Firebase (convertible to MongoDB/Express)

APIs: Maps, SMS, Location, Emergency Services

Database Options: Firestore / MongoDB

Deployment: Firebase Hosting / Vercel (for web variant)

## 📂 Functional Flowchart

<img width="400" height="800" alt="image" src="https://github.com/user-attachments/assets/5802fd16-b583-4853-b241-64652e2ba90f" />

## 🎨 UI Preview
# femigo
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Femigo Location UI</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-[#0e0c18] text-white font-sans min-h-screen p-4">

  <!-- Header -->
  <div class="mb-6">
    <h1 class="text-2xl font-bold flex items-center gap-2">
      <span class="text-white">&larr;</span> Femigo <span class="text-pink-500">❤</span>
    </h1>
  </div>

  <!-- Input Section -->
  <div class="space-y-3">
    <div class="bg-[#1a1a2e] p-3 rounded-xl flex items-center justify-between">
      <span>📍</span>
      <input type="text" class="bg-transparent w-full ml-2 text-sm placeholder-gray-400 focus:outline-none" placeholder='26°12′31.4″N 78°11′28.2″E'>
      <button>🔁</button>
    </div>

    <div class="bg-[#1a1a2e] p-3 rounded-xl flex items-center justify-between">
      <span>📌</span>
      <input type="text" class="bg-transparent w-full ml-2 text-sm placeholder-gray-400 focus:outline-none" placeholder='Rolex Square Commercial Cplx, Bhaskar Lane, City Center'>
    </div>

    <!-- Travel Modes -->
    <div class="bg-[#1a1a2e] p-2 rounded-xl flex justify-between items-center">
      <button class="w-1/4 text-center text-gray-400">🚗</button>
      <button class="w-1/4 text-center text-gray-400">🚴</button>
      <button class="w-1/4 text-center text-gray-400">🚌</button>
      <button class="w-1/4 text-center bg-pink-600 text-white font-bold rounded-xl py-2">🚶‍♀</button>
    </div>
  </div>

  <!-- Select a Route -->
  <div class="mt-6">
    <h2 class="text-lg font-semibold mb-2">Select a Route</h2>
    
    <!-- AI Recommendation -->
    <div class="bg-green-700/70 p-3 rounded-xl mb-3">
      <p class="font-bold text-sm">AI Recommendation</p>
      <p class="text-xs text-white/80">This is the primary suggested route.</p>
    </div>

    <!-- Route Card -->
    <div class="bg-[#2c002c] p-4 rounded-xl relative border border-pink-800">
      <div class="absolute right-2 top-2 bg-green-600 px-2 text-xs rounded text-white">Recommended</div>
      <h3 class="font-bold text-lg mb-1">Route 1</h3>
      <p class="text-sm text-gray-300 mb-2">0.5 km · 7 mins</p>

      <div class="grid grid-cols-2 gap-2 text-xs text-white/80">
        <p>⚠ Moderate</p>
        <p>⚠ Data unavailable</p>
        <p>🌓 Partially-lit</p>
        <p>🚦 Medium Traffic</p>
        <p>💬 0 Reviews</p>
      </div>

      <button class="bg-purple-600 text-white px-3 py-1 rounded-lg text-xs mt-3">More Info</button>
    </div>
  </div>

  <!-- MAP Section -->
  <div class="mt-6">
    <h2 class="text-lg font-semibold mb-2">Destination</h2>

    <div class="space-y-3">
      <div class="bg-[#1a1a2e] p-3 rounded-xl flex items-center justify-between">
        <span>📍</span>
        <input type="text" class="bg-transparent w-full ml-2 text-sm placeholder-gray-400 focus:outline-none" placeholder='Your Location'>
        <button>🔁</button>
      </div>

      <div class="bg-[#1a1a2e] p-3 rounded-xl flex items-center justify-between">
        <span>📌</span>
        <input type="text" class="bg-transparent w-full ml-2 text-sm placeholder-gray-400 focus:outline-none" placeholder='Destination or coordinates'>
      </div>

      <div class="bg-[#1a1a2e] p-2 rounded-xl flex justify-between items-center">
        <button class="w-1/4 text-center text-gray-400">🚗</button>
        <button class="w-1/4 text-center text-gray-400">🚴</button>
        <button class="w-1/4 text-center text-gray-400">🚌</button>
        <button class="w-1/4 text-center bg-pink-600 text-white font-bold rounded-xl py-2">🚶‍♀</button>
      </div>

      <!-- Google Maps Embed -->
      <div class="overflow-hidden rounded-xl mt-4">
        <iframe class="w-full h-60 rounded-xl"
          src="https://maps.google.com/maps?q=Indore&t=&z=13&ie=UTF8&iwloc=&output=embed"
          frameborder="0" allowfullscreen loading="lazy">
        </iframe>
      </div>

      <!-- Start Button -->
      <button class="w-full bg-pink-600 text-white font-semibold py-3 mt-3 rounded-xl opacity-60" disabled>
        START
      </button>

      <!-- Bottom Buttons -->
      <div class="flex justify-between gap-3 mt-4">
        <button class="w-1/2 bg-[#1a1a2e] py-3 rounded-xl text-sm text-white">📤 Share Live Location</button>
        <button class="w-1/2 bg-[#1a1a2e] py-3 rounded-xl text-sm text-white">🛰 Track Me</button>
      </div>
    </div>
  </div>

</body>
</html>




