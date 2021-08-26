<template>
  <div class="container mx-auto p-3">
    <div class="grid grid-flow-col grid-cols-3 h-screen">
      <div class="col-span-2">
        <div class="flex flex-col h-full justify-center place-items-center">
          <h1>Talk to your tank like Humans</h1>
          <h3 class="font-light mt-5">Homepage subtext goes here</h3>
          <dropdown cls="px-3 py-1 border-0 shadow-none mt-5" right icon divider>
            <template #icon>
              <avatar
                imageSrc="https://uifaces.co/our-content/donated/6MWH9Xi_.jpg"
                userImage
                size="xs"
                class="mr-2"
                cls="positive"
              ></avatar>Karthick Thangaraju
            </template>
            <div class="p-4">
              <b>karthickt@teezle.com</b>
              <p class="text-gray-500">Last login: Yesterday</p>
            </div>
            <div>
              <dropdown-item link="/">My Profile</dropdown-item>
              <dropdown-item link="/preferences">Preference</dropdown-item>
            </div>
            <dropdown-item>Logout</dropdown-item>
          </dropdown>
        </div>
      </div>
      <div class="w-full mx-auto">
        <h4>Login</h4>
        <p>Subtext</p>
        <div class>
          <form class="space-y-4">
            <div>
              <p>Email address</p>
              <input type="text" class="w-full" />
            </div>
            <div>
              <p>Password</p>
              <input type="text" class="w-full" />
            </div>
            <div>
              <btn class="dark w-full">Login</btn>
            </div>
            <dropdown cls="px-3 py-1 border-0 shadow-none mt-5" right icon divider>
              <template #icon>
                <avatar
                  imageSrc="https://uifaces.co/our-content/donated/6MWH9Xi_.jpg"
                  userImage
                  size="xs"
                  class="mr-2"
                  cls="positive"
                ></avatar>Karthick Thangaraju
              </template>
              <div class="p-4">
                <b>karthickt@teezle.com</b>
                <p class="text-gray-500">Last login: Yesterday</p>
              </div>
              <div>
                <dropdown-item link="/">My Profile</dropdown-item>
                <dropdown-item link="/preferences">Preference</dropdown-item>
              </div>
              <dropdown-item>Logout</dropdown-item>
            </dropdown>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="postcss" scoped>
</style>