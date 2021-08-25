<template>
  <div class="container mx-auto my-5">
    <h1>H8 UI Elements with Tailwind CSS</h1>
    <hr class="my-3" />
    <div class="space-y-4 divide-y divide-gray-100">
      <div>
        <h4 class="my-3">Buttons</h4>
        <btn @click="clickHandler">Open Commands Dictionary</btn>
        <btn class="dark">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-5 w-5 mr-1 inline-block"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="1.6"
              d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z"
            />
          </svg>
          Post Message
        </btn>
      </div>

      <div class>
        <h4 class="my-3">Dropdowns</h4>
        <div class="flex space-x-3 align-bottom">
          <dropdown label="Open Commands Dictionary">
            <div class="py-1">
              <dropdown-item>
                <p>Signed in as</p>
                <b>johnmathew@email.com</b>
              </dropdown-item>
            </div>
            <div class="py-1">
              <dropdown-item>Account Settings</dropdown-item>
              <dropdown-item>Support</dropdown-item>
              <dropdown-item>License</dropdown-item>
            </div>
            <div class="py-1">
              <dropdown-item>Option 1</dropdown-item>
              <dropdown-item>Option 1</dropdown-item>
            </div>
            <div class="py-1">
              <dropdown-item>Option 1</dropdown-item>
              <dropdown-item>Option 1</dropdown-item>
            </div>
            <div>
              <dropdown-item>Account Settings</dropdown-item>
              <dropdown-item>Support</dropdown-item>
              <dropdown-item>License</dropdown-item>
            </div>
            <div>
              <dropdown-item>Sign Out</dropdown-item>
            </div>
          </dropdown>
          <dropdown cls="dark" label="All Accounts" divider>
            <div class="p-4 text-gray-500 text-xs">
              <p class="text-primary-700 font-bold text-sm">Info</p>For a project template project, you should see your project template listed in the New Project dialog (File > New > Project).
            </div>
            <dropdown-item>Project Settings</dropdown-item>
            <div>
              <dropdown-item>Account Settings</dropdown-item>
              <dropdown-item>Support</dropdown-item>
              <dropdown-item>License</dropdown-item>
            </div>
            <div>
              <dropdown-item>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-4 w-4 inline-block align-text-bottom"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M17 16l4-4m0 0l-4-4m4 4H7m6 4v1a3 3 0 01-3 3H6a3 3 0 01-3-3V7a3 3 0 013-3h4a3 3 0 013 3v1"
                  />
                </svg>
                Sign Out
              </dropdown-item>
            </div>
          </dropdown>
          <dropdown cls="primary" label="All Accounts" divider>
            <div class="p-4 text-gray-500 text-xs">
              <p class="text-primary-700 font-bold text-sm">Info</p>For a project template project, you should see your project template listed in the New Project dialog (File > New > Project).
            </div>
            <dropdown-item>Project Settings</dropdown-item>
            <div>
              <dropdown-item>Account Settings</dropdown-item>
              <dropdown-item>Support</dropdown-item>
              <dropdown-item>License</dropdown-item>
            </div>
            <div>
              <dropdown-item>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-4 w-4 inline-block align-text-bottom"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M17 16l4-4m0 0l-4-4m4 4H7m6 4v1a3 3 0 01-3 3H6a3 3 0 01-3-3V7a3 3 0 013-3h4a3 3 0 013 3v1"
                  />
                </svg>
                Sign Out
              </dropdown-item>
            </div>
          </dropdown>
          <dropdown label="All Accounts" divider>
            <div class="p-4 text-gray-500 text-xs">
              <p class="text-primary-700 font-bold text-sm">Info</p>For a project template project, you should see your project template listed in the New Project dialog (File > New > Project).
            </div>
            <dropdown-item>Project Settings</dropdown-item>
            <div>
              <dropdown-item>Account Settings</dropdown-item>
              <dropdown-item>Support</dropdown-item>
              <!-- <dropdown-item> -->
              <!-- <dropdown label="License" class="w-full" divider></dropdown> -->
              <!-- </dropdown-item> -->
            </div>
            <div>
              <dropdown-item class="text-red-600">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-4 w-4 inline-block align-text-bottom"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M17 16l4-4m0 0l-4-4m4 4H7m6 4v1a3 3 0 01-3 3H6a3 3 0 01-3-3V7a3 3 0 013-3h4a3 3 0 013 3v1"
                  />
                </svg>
                Sign Out
              </dropdown-item>
            </div>
          </dropdown>
          <dropdown label="Info" hideTrailingIcon icon>
            <template #icon>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-5 w-5"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
                />
              </svg>
            </template>
            <div class="p-4 text-gray-500 text-xs">
              <p class="text-primary-700 font-bold text-sm">Info</p>For a project template project, you should see your project template listed in the New Project dialog (File > New > Project).
            </div>
          </dropdown>
        </div>
      </div>
      <div>
        <h4 class="my-3">Badges</h4>
        <div class="space-y-2">
          <div class="flex space-x-1">
            <badge class="negative" closable @closed="badgeClosed">Speeding</badge>
            <badge class="primary">Badge</badge>
            <badge class="secondary">Scheduled Message</badge>
            <badge class="info">Requested</badge>
            <badge class="positive">Discharge Start</badge>
            <badge class="negative">Modbus Error</badge>
          </div>
          <div class="flex space-x-1">
            <badge class="dark">Badge</badge>
            <badge class="primary filled">Badge</badge>
            <badge class="secondary filled">Badge</badge>
            <badge class="info filled">Badge</badge>
            <badge class="positive filled">Badge</badge>
            <badge class="negative filled">Badge</badge>
          </div>
          <div class="flex place-items-center relative space-x-1">
            <Badge class closable @closed="badgeClosed">Out of Service</Badge>
            <Badge class="primary" closable @closed="badgeClosed">Out of Service</Badge>
            <Badge class="positive filled" closable @closed="badgeClosed">Out of Service</Badge>
            <badge class="primary">Badge</badge>
            <badge class="secondary">Badge</badge>
            <badge class="info">Badge</badge>
            <badge class="positive">Badge</badge>
            <badge class="negative">Badge</badge>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  component: {},
  methods: {
    clickHandler() {
      alert("clicked");
    },
    badgeClosed($dom, data) {
      $dom.remove();
    },
  },
};
</script>

<style lang="postcss" scoped>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
</style>