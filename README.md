<!DOCTYPE html>
<html lang="en" class="h-full">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Hungarian State Railways</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" rel="stylesheet">
  <style>
    body { font-family: system-ui, -apple-system, sans-serif; }
    .máv-logo { filter: brightness(1.1); }
  </style>
</head>
<body class="bg-[#003087] min-h-screen text-white">

  <!-- Header -->
  <div class="bg-gradient-to-r from-blue-900 to-blue-800 py-3 px-6 flex items-center justify-between shadow-lg">
    <h1 class="text-2xl font-bold tracking-wider">Hungarian State Railways</h1>
    <button class="text-white hover:text-red-400 text-3xl font-bold">✕</button>
  </div>

  <div class="max-w-7xl mx-auto p-6 grid grid-cols-1 lg:grid-cols-12 gap-6">

    <!-- Left Panel - MÁV-START -->
    <div class="lg:col-span-7 bg-white text-gray-900 rounded-2xl shadow-2xl overflow-hidden">
      
      <!-- Blue Header -->
      <div class="bg-gradient-to-r from-blue-600 to-blue-700 px-8 py-5 flex items-center gap-4">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0f/M%C3%81V_logo.svg/512px-M%C3%81V_logo.svg.png" 
             alt="MÁV" class="h-14 máv-logo">
        <div>
          <span class="text-3xl font-bold tracking-tighter">MÁV-START</span>
        </div>
        <div class="ml-auto text-2xl font-semibold">Welcome!</div>
      </div>

      <!-- Info Box -->
      <div class="bg-blue-700 text-white p-6 text-sm leading-relaxed">
        <div class="flex gap-3">
          <div class="text-3xl">ℹ️</div>
          <div>
            <strong>Please be informed that purchasing a ticket does not require any form of payment.</strong><br>
            There is no currency real or virtual that you need to spend.<br>
            All tickets are completely free of charge, and you will never be asked to pay for them.<br><br>
            We kindly ask that you obtain your ticket through the correct method to ensure a smooth journey.
          </div>
        </div>
      </div>

      <!-- Form Section -->
      <div class="p-8">
        <div class="grid grid-cols-2 gap-8">
          <!-- From / To -->
          <div>
            <label class="block text-sm font-medium mb-1">From:</label>
            <input type="text" value="Nádormaros" 
                   class="w-full border border-gray-300 rounded-lg px-4 py-3 text-lg focus:outline-none focus:border-blue-500">
            
            <label class="block text-sm font-medium mt-6 mb-1">To:</label>
            <input type="text" value="Dobóvárad" 
                   class="w-full border border-gray-300 rounded-lg px-4 py-3 text-lg focus:outline-none focus:border-blue-500">
            
            <div class="mt-4 bg-blue-50 border border-blue-200 rounded-xl p-4 text-sm text-blue-800">
              You can copy paste the station's name from the list!
            </div>
          </div>

          <!-- Calendar -->
          <div>
            <label class="block text-sm font-medium mb-2">When</label>
            <div class="flex justify-between items-center mb-2">
              <button class="text-blue-600 hover:text-blue-800 text-2xl">❮❮</button>
              <div class="text-xl font-semibold text-center">2025. June</div>
              <button class="text-blue-600 hover:text-blue-800 text-2xl">❯❯</button>
            </div>

            <!-- Calendar Grid -->
            <table class="w-full text-center border-collapse">
              <thead>
                <tr class="text-xs text-gray-500">
                  <th class="py-2">Monday</th>
                  <th>Tuesday</th>
                  <th>Wednesday</th>
                  <th>Thursday</th>
                  <th>Friday</th>
                  <th>Saturday</th>
                  <th>Sunday</th>
                </tr>
              </thead>
              <tbody class="text-lg">
                <tr><td class="py-2"></td><td></td><td></td><td></td><td></td><td class="text-orange-500">1</td></tr>
                <tr><td class="py-2">2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td></tr>
                <tr><td class="py-2">9</td><td>10</td><td>11</td><td>12</td><td>13</td><td>14</td><td>15</td></tr>
                <tr><td class="py-2">16</td><td>17</td><td>18</td><td>19</td><td>20</td><td>21</td><td>22</td></tr>
                <tr><td class="py-2">23</td><td>24</td><td>25</td><td>26</td><td>27</td><td>28</td><td>29</td></tr>
                <tr><td class="py-2">30</td></tr>
              </tbody>
            </table>
          </div>
        </div>

        <!-- Recruitment Box -->
        <div class="mt-8 bg-white border border-gray-200 rounded-2xl p-6 flex gap-5 items-start">
          <div class="bg-blue-100 text-blue-600 p-4 rounded-2xl">
            👮‍♂️
          </div>
          <div class="text-sm">
            <strong>Ever wanted to work on the railways?</strong><br>
            Join us as a train driver, dispatcher, or ticket inspector and be part of keeping the journey on track!<br>
            <span class="text-blue-600 font-medium">Start your railway adventure today!</span>
          </div>
        </div>

        <!-- Purchase Button -->
        <button onclick="alert('Ticket purchased! 🎟️ (This is a recreation)')" 
                class="mt-8 w-full bg-gradient-to-r from-orange-500 to-orange-600 hover:from-orange-600 hover:to-orange-700 text-white font-bold text-xl py-5 rounded-2xl shadow-lg transition">
          Purchase
        </button>

        <!-- Warning -->
        <div class="mt-8 text-red-600 text-sm leading-relaxed">
          <strong>Dear Passenger,</strong><br>
          Please make sure to double-check where you are purchasing your ticket from!<br>
          If the ticket is incorrect, you may be removed from the train.<br>
          <strong>Tickets are non-refundable under any circumstances.</strong>
        </div>
      </div>
    </div>

    <!-- Right Panel - Ticket -->
    <div class="lg:col-span-5">
      <div class="bg-white text-gray-900 rounded-2xl shadow-2xl overflow-hidden">
        
        <!-- Ticket Header -->
        <div class="bg-white border-b flex justify-between items-center px-6 py-4">
          <div class="flex items-center gap-3">
            <div class="text-3xl">🚂</div>
            <div>
              <div class="font-bold text-lg">MENETJEGY</div>
              <div class="text-xs text-gray-500">1120 Ft</div>
            </div>
          </div>
          <div class="text-right text-sm">
            <div class="font-medium">Áfát. 71,26%</div>
          </div>
        </div>

        <!-- Ticket Content -->
        <div class="p-6 space-y-6">
          <div>
            <div class="text-sm text-gray-500">Nádormaros</div>
            <div class="font-bold text-xl">Dobóvárad (-)</div>
            <div class="text-sm text-gray-500">Teljesárú</div>
          </div>

          <div class="grid grid-cols-2 gap-4 text-sm">
            <div>
              <div class="text-gray-500">Érv.:</div>
              <div class="font-semibold">2025. 7. 21. 17:25</div>
              <div class="font-semibold">2025. 7. 21. 21:25</div>
            </div>
            <div class="text-right">
              <div class="text-gray-500">*1 db</div>
              <div class="text-gray-500">2. osztály</div>
            </div>
          </div>

          <div class="border-t border-dashed pt-4">
            <div class="text-xs text-gray-500">Egy útra</div>
            <div class="font-mono text-sm">MÁV/0/53,0</div>
          </div>

          <!-- QR Code -->
          <div class="flex justify-center my-4">
            <div class="bg-black p-4 rounded-xl">
              <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=CTV%205501511X200092589%20CA%2026230866%201740%205501511-504%20JK3-186" 
                   alt="QR Code" class="w-40 h-40">
            </div>
          </div>

          <div class="text-[10px] font-mono text-center text-gray-600 leading-tight">
            CTV 5501511X200092589 CA<br>
            26230866 1740 5501511-504<br>
            JK3-186
          </div>
        </div>

        <!-- Stations List -->
        <div class="bg-gray-900 text-white p-6">
          <div class="uppercase text-xs tracking-widest mb-3 text-gray-400">Stations:</div>
          <ul class="space-y-1 text-sm">
            <li>Nádormaros</li>
            <li>Tímárháza</li>
            <li>Tornyos mh</li>
            <li>Dobóvárad</li>
            <li>Rálospuszta</li>
            <li>Mecsekháza</li>
          </ul>
        </div>
      </div>
    </div>
  </div>

  <!-- Bottom Navigation -->
  <div class="fixed bottom-0 left-0 right-0 bg-white border-t py-3 px-6 text-xs text-gray-700 shadow-2xl">
    <div class="max-w-7xl mx-auto flex items-center justify-between text-center">
      <div class="flex-1 flex flex-col items-center">
        🌐 <span class="block mt-1">English</span>
      </div>
      <div class="flex-1 flex items-center justify-center gap-2 text-blue-600 font-medium">
        <span class="text-xl">①</span> Select Route
      </div>
      <div class="flex-1 flex items-center justify-center gap-2">
        <span class="text-xl">②</span> Review
      </div>
      <div class="flex-1 flex items-center justify-center gap-2">
        <span class="text-xl">✅</span> Confirm
      </div>
      <div class="flex-1 flex items-center justify-center gap-2">
        <span class="text-xl">④</span> Collect Ticket
      </div>
    </div>
  </div>

</body>
</html>
