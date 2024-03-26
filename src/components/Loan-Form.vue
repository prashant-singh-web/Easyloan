<script>
export default {}
</script>
<template>
  <div class="w-full grid place-items-center">
    <div class="w-full md:w-[80%] lg:w-3/4 place-items-center p-5 gap-10 grid grid-cols-1">
      <div class="w-full grid grid-cols-4 gap-6">
        <!-- first name -->
        <div class="w-full col-span-4 sm:col-span-2 md:col-span-4 lg:col-span-2 flex flex-col">
          <label for="first_name" class="lable-style">First name <sup>*</sup></label>
          <input
            type="text"
            required
            id="first_name"
            placeholder="Enter first name"
            class="input-style"
          />
        </div>
        <!-- last name -->
        <div class="w-full col-span-4 sm:col-span-2 md:col-span-4 lg:col-span-2 flex flex-col">
          <label for="last_name" class="lable-style">Last name <sup>*</sup></label>
          <input
            type="text"
            required
            id="last_name"
            placeholder="Enter last name"
            class="input-style"
          />
        </div>
        <!-- email input -->
        <div class="w-full col-span-4 sm:col-span-2 md:col-span-4 lg:col-span-2 flex flex-col">
          <label for="contact_email" class="lable-style">Email <sup>*</sup></label>
          <input
            type="email"
            required
            id="contact_email"
            placeholder="Enter your email"
            class="input-style"
          />
        </div>
        <!-- contact number input -->
        <div class="w-full col-span-4 sm:col-span-2 md:col-span-4 lg:col-span-2 flex flex-col">
          <label for="contact_number" class="lable-style">Number <sup>*</sup></label>
          <input
            type="text"
            required
            id="contact_number"
            placeholder="Enter your number"
            class="input-style"
          />
        </div>
        <!-- loan amount input -->
        <div class="w-full col-span-4 sm:col-span-2 md:col-span-4 lg:col-span-2 flex flex-col">
          <label for="loan_amount" class="lable-style">Loan Amount <sup>*</sup></label>
          <input
            type="text"
            required
            id="loan_amount"
            placeholder="Enter loan amount"
            class="input-style"
          />
        </div>
        <div class="w-full col-span-4 sm:col-span-2 md:col-span-4 lg:col-span-2 flex flex-col">
          <label for="loan_purpose" class="lable-style">Purpose of loan <sup>*</sup></label>
          <input
            type="text"
            required
            id="loan_purpose"
            placeholder="Enter loan purpose"
            class="input-style"
          />
        </div>
        <div class="col-span-4 w-full flex flex-row items-center">
          <p class="lable-style">Gender <sup>*</sup>:</p>
          <div class="flex flex-row">
            <div class="flex flex-row items-center space-x-2 pl-2">
              <label for="male_radio" class="lable-style my-auto">Male :</label>
              <input name="gender" type="radio" id="male_radio" />
            </div>
            <div class="flex flex-row items-center space-x-2 pl-2">
              <label for="female_radio" class="lable-style my-auto">Female :</label>
              <input type="radio" id="female_radio" name="gender" />
            </div>
          </div>
        </div>
        <button
          class="col-span-2 sm:col-span-1 md:col-span-2 lg:col-span-1 border border-sky-500 py-2 text-gray-500 text-sm hover:bg-sky-500 hover:text-white ease-in-out duration-200"
        >
          Send
        </button>
      </div>
    </div>
  </div>
</template>
<style>
.input-style {
  @apply w-full border border-gray-300 outline-none focus-within:border-sky-500 p-2 rounded-sm text-sm shadow;
}
.lable-style {
  @apply text-sm mb-2 text-gray-500;
}
</style>
