<script>
export default {}
</script>
<template>
  <div class="w-full grid place-items-center">
    <h1 class="text-2xl font-bold">Contact Form</h1>
    <div
      class="w-full md:w-[80%] lg:w-3/4 place-items-center p-5 gap-10 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-[60%_40%]"
    >
      <div class="w-full grid grid-cols-4 gap-3">
        <div class="w-full col-span-4 flex flex-col">
          <label for="contactMessage" class="text-sm mb-2 text-gray-500">Enter your message</label>
          <textarea
            name="hii"
            id="contactMessage"
            placeholder="Enter your message"
            rows="6"
            class="w-full border border-gray-300 outline-none focus-within:border-sky-500 p-3 rounded-sm text-sm"
          ></textarea>
        </div>
        <div class="w-full col-span-4 sm:col-span-2 md:col-span-4 lg:col-span-2 flex flex-col">
          <label for="contactName" class="text-sm mb-2 text-gray-500">Your name</label>
          <input
            type="text"
            required
            id="contactName"
            placeholder="Enter your name"
            class="w-full border border-gray-300 outline-none focus-within:border-sky-500 p-2 rounded-sm text-sm"
          />
        </div>
        <div class="w-full col-span-4 sm:col-span-2 md:col-span-4 lg:col-span-2 flex flex-col">
          <label for="contactEmail" class="text-sm mb-2 text-gray-500">Your email</label>
          <input
            type="email"
            required
            id="contactEmail"
            placeholder="Enter your email"
            class="w-full border border-gray-300 outline-none focus-within:border-sky-500 p-2 rounded-sm text-sm"
          />
        </div>
        <div class="w-full col-span-4 flex flex-col">
          <label for="contactSubject" class="text-sm mb-2 text-gray-500">Subject</label>
          <input
            type="text"
            required
            id="contactSubject"
            placeholder="Enter your subject"
            class="w-full border border-gray-300 outline-none focus-within:border-sky-500 p-2 rounded-sm text-sm"
          />
        </div>
        <button
          class="col-span-2 sm:col-span-1 md:col-span-2 lg:col-span-1 border border-sky-500 py-2 text-gray-500 text-sm hover:bg-sky-500 hover:text-white ease-in-out duration-200"
        >
          Send
        </button>
      </div>
      <div class="w-full flex flex-col space-y-4 justify-evenly h-full">
        <div class="flex flex-row items-center space-x-4">
          <i class="fa-solid text-3xl p-2 fa-house text-sky-500"></i>
          <div class="flex flex-col">
            <p class="text-base font-semibold text-gray-800/75">Jaunpur,Uttar Predash</p>
            <p class="text-sm text-gray-500">222136</p>
          </div>
        </div>
        <div class="flex flex-row items-center space-x-4">
          <i class="fa-solid text-3xl p-2 fa-phone text-sky-500"></i>
          <div class="flex flex-col">
            <p class="text-base font-semibold text-gray-800/75">+91 7652021778</p>
            <p class="text-sm text-gray-500">Mon to Fri 9am to 6pm</p>
          </div>
        </div>
        <div class="flex flex-row items-center space-x-4">
          <i class="fa-solid text-3xl p-2 fa-envelope text-sky-500"></i>
          <div class="flex flex-col">
            <p class="text-base font-semibold text-gray-800/75">prashantsingh7559@gmail.com</p>
            <p class="text-sm text-gray-500">Mon to Fri 9am to 6pm</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
