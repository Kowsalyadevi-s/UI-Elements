<template>
  <div class="container mx-auto my-5">
    <h1>H8 UI Elements with Tailwind CSS</h1>
    <hr class="my-3" />
    <div class="space-y-12 divide-y divide-gray-100 mb-12">
      <div class="space-y-3">
        <h4 class="my-3">Buttons</h4>
        <div>
          <Btn2 @click="clickHandler">Open Commands Dictionary</Btn2>
          <Btn2 class="default">Open Commands Dictionary</Btn2>
          <Btn2 class="dark">
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
          </Btn2>
        </div>
        <div>
          <Btn2 class="default rounded-full">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 inline-block"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M12 4v16m8-8H4"
              />
            </svg>
          </Btn2>

          <Btn2 class="primary rounded-full">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 inline-block"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </Btn2>
          <Btn2 class="dark rounded-full">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 inline-block"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"
              />
            </svg>
          </Btn2>
        </div>
      </div>

      <div>
        <h4 class="my-3">Grouped Buttons</h4>
        <div class="flex space-x-2">
          <btn-group>
            <Btn2>Left</Btn2>
            <Btn2>Center</Btn2>
            <Btn2>Right</Btn2>
          </btn-group>

          <btn-group>
            <Btn2 class="dark">All Assets</Btn2>
            <Btn2 variant="default">Reporting</Btn2>
            <Btn2 variant="default">Non Reporting</Btn2>
          </btn-group>

          <btn-group>
            <Btn2>
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
                  d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2"
                />
              </svg>
            </Btn2>
            <Btn2>
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
                  d="M12 10v6m0 0l-3-3m3 3l3-3m2 8H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"
                />
              </svg>
            </Btn2>
            <Btn2>
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
                  d="M3 4a1 1 0 011-1h16a1 1 0 011 1v2.586a1 1 0 01-.293.707l-6.414 6.414a1 1 0 00-.293.707V17l-4 4v-6.586a1 1 0 00-.293-.707L3.293 7.293A1 1 0 013 6.586V4z"
                />
              </svg>
            </Btn2>
          </btn-group>

          <btn-group variant="primary">
            <Btn2>
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
                  d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2"
                />
              </svg>
              Code
            </Btn2>
            <Btn2>
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
                  d="M12 10v6m0 0l-3-3m3 3l3-3m2 8H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"
                />
              </svg>
              Download
            </Btn2>
          </btn-group>
        </div>
      </div>

      <div class>
        <h4 class="my-3">Dropdowns</h4>
        <div class="flex space-x-3 align-bottom">
          <dropdown label="Open Commands Dictionary">
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
          <dropdown cls="default" label="Open Commands Dictionary">
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
          <dropdown cls="default" label="Pay with" divider right>
            <dropdown-item class="flex space-x-2">
              <div>
                <svg
                  class="w-6 h-6"
                  role="img"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <title>Stripe</title>
                  <path
                    d="M13.976 9.15c-2.172-.806-3.356-1.426-3.356-2.409 0-.831.683-1.305 1.901-1.305 2.227 0 4.515.858 6.09 1.631l.89-5.494C18.252.975 15.697 0 12.165 0 9.667 0 7.589.654 6.104 1.872 4.56 3.147 3.757 4.992 3.757 7.218c0 4.039 2.467 5.76 6.476 7.219 2.585.92 3.445 1.574 3.445 2.583 0 .98-.84 1.545-2.354 1.545-1.875 0-4.965-.921-6.99-2.109l-.9 5.555C5.175 22.99 8.385 24 11.714 24c2.641 0 4.843-.624 6.328-1.813 1.664-1.305 2.525-3.236 2.525-5.732 0-4.128-2.524-5.851-6.594-7.305h.003z"
                  />
                </svg>
              </div>
              <div>
                <b>Stripe</b>
                <p class="text-gray-400 text-xs">Pay with your stripe account</p>
              </div>
            </dropdown-item>
            <dropdown-item class="flex space-x-2">
              <div>
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 48 48" class="w-6 h-6">
                  <path
                    fill="#3F51B5"
                    d="M45,35c0,2.209-1.791,4-4,4H7c-2.209,0-4-1.791-4-4V13c0-2.209,1.791-4,4-4h34c2.209,0,4,1.791,4,4V35z"
                  />
                  <path fill="#FFC107" d="M30 14A10 10 0 1 0 30 34A10 10 0 1 0 30 14Z" />
                  <path
                    fill="#FF3D00"
                    d="M22.014,30c-0.464-0.617-0.863-1.284-1.176-2h5.325c0.278-0.636,0.496-1.304,0.637-2h-6.598C20.07,25.354,20,24.686,20,24h7c0-0.686-0.07-1.354-0.201-2h-6.598c0.142-0.696,0.359-1.364,0.637-2h5.325c-0.313-0.716-0.711-1.383-1.176-2h-2.973c0.437-0.58,0.93-1.122,1.481-1.595C21.747,14.909,19.481,14,17,14c-5.523,0-10,4.477-10,10s4.477,10,10,10c3.269,0,6.162-1.575,7.986-4H22.014z"
                  />
                </svg>
              </div>
              <div>
                <b>Mastercard</b>
                <p class="text-gray-400 text-xs">Pay with your mastercard account</p>
              </div>
            </dropdown-item>
            <dropdown-item class="flex space-x-2">
              <div>
                <svg
                  role="img"
                  class="w-6 h-6"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <title>PayPal</title>
                  <path
                    d="M7.076 21.337H2.47a.641.641 0 0 1-.633-.74L4.944.901C5.026.382 5.474 0 5.998 0h7.46c2.57 0 4.578.543 5.69 1.81 1.01 1.15 1.304 2.42 1.012 4.287-.023.143-.047.288-.077.437-.983 5.05-4.349 6.797-8.647 6.797h-2.19c-.524 0-.968.382-1.05.9l-1.12 7.106zm14.146-14.42a3.35 3.35 0 0 0-.607-.541c-.013.076-.026.175-.041.254-.93 4.778-4.005 7.201-9.138 7.201h-2.19a.563.563 0 0 0-.556.479l-1.187 7.527h-.506l-.24 1.516a.56.56 0 0 0 .554.647h3.882c.46 0 .85-.334.922-.788.06-.26.76-4.852.816-5.09a.932.932 0 0 1 .923-.788h.58c3.76 0 6.705-1.528 7.565-5.946.36-1.847.174-3.388-.777-4.471z"
                  />
                </svg>
              </div>
              <div>
                <b>Paypal</b>
                <p class="text-gray-400 text-xs">Pay with your paypal account</p>
              </div>
            </dropdown-item>
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
      <!-- Badge -->
      <div>
        <h4 class="my-3">Badges</h4>
        <div class="space-y-3">
          <div class="space-x-1">
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
            <Badge
              class="flex flex-wrap content-center primary"
              closable
              @closed="badgeClosed"
            >Out of Service</Badge>
            <Badge class="primary" closable @closed="badgeClosed">Out of Service</Badge>
            <Badge class="positive filled" closable @closed="badgeClosed">Out of Service</Badge>
            <badge class="primary">Badge</badge>
            <badge class="secondary">Badge</badge>
            <badge class="info">Badge</badge>
            <badge class="positive">Badge</badge>
            <badge class="negative">Badge</badge>
          </div>
          <div class="flex space-x-1">
            <badge class="negative rounded">Speeding</badge>
            <badge class="primary rounded">Badge</badge>
            <badge class="secondary rounded">Scheduled Message</badge>
            <badge class="info filled rounded">Requested</badge>
            <badge class="positive rounded">Discharge Start</badge>
            <badge class="negative rounded">Modbus Error</badge>
          </div>
          <div class="flex place-items-center relative space-x-1">
            <badge class status statusClass="negative">Badge</badge>
            <badge status statusClass="warning">Badge</badge>
            <badge status statusClass="info">Badge</badge>
            <badge status statusClass="positive">Badge</badge>
            <badge status>Badge</badge>
          </div>
        </div>
      </div>
      <!-- END: Badge -->
      <!-- Avatar -->
      <div class="flex flex-col">
        <h4 class="my-3">Avatar</h4>
        <div class="space-y-3">
          <div class="flex space-x-2 place-items-center">
            <Avatar
              size="xs"
              userImage
              imageSrc="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
            ></Avatar>
            <Avatar
              size="sm"
              userImage
              imageSrc="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
            ></Avatar>
            <Avatar
              userImage
              imageSrc="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
            ></Avatar>
            <Avatar
              size="lg"
              userImage
              imageSrc="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
            ></Avatar>
            <Avatar
              size="xl"
              userImage
              imageSrc="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
            ></Avatar>
            <Avatar
              size="xxl"
              userImage
              imageSrc="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
            ></Avatar>
          </div>
          <div class="flex space-x-1 place-items-center">
            <Avatar cls="info" size="xs" initial="TK"></Avatar>
            <Avatar cls="warning" size="sm" initial="TK"></Avatar>
            <Avatar size="sm" initial="TK"></Avatar>
            <Avatar cls="positive" initial="TK"></Avatar>
            <Avatar cls="negative" size="lg" initial="TK"></Avatar>
            <Avatar cls="secondary" size="xl" initial="TK"></Avatar>
            <Avatar cls="primary" size="xxl" initial="TK"></Avatar>
          </div>
          <div class="flex space-x-1 place-items-center">
            <Avatar cls="info" size="sm" initial="K"></Avatar>
            <Avatar cls="warning" size="sm" initial="K"></Avatar>
            <Avatar size="sm" initial="K"></Avatar>
            <Avatar cls="positive" size="sm" initial="K"></Avatar>
            <Avatar cls="negative" size="sm" initial="K"></Avatar>
            <Avatar cls="secondary" size="sm" initial="K"></Avatar>
            <Avatar cls="primary" size="sm" initial="K"></Avatar>
          </div>
        </div>
      </div>
      <!-- END: Avatar -->
      <!-- Profile Card -->
      <div class="flex flex-col">
        <h4 class="my-3">Profile Card</h4>
        <div class="flex space-x-2 my-5 place-items-center">
          <Btn2 class="flex place-items-center space-x-1">
            <Avatar
              class="flex place-content-center"
              size="xs"
              userImage
              imageSrc="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
            ></Avatar>
            <p class="font-medium">John Mathew</p>
          </Btn2>
          <dropdown right icon divider>
            <template #icon>
              <avatar
                imageSrc="https://uifaces.co/our-content/donated/6MWH9Xi_.jpg"
                userImage
                size="xs"
                class="flex mr-2 place-content-center"
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
          <dropdown right icon divider>
            <template #icon>
              <avatar initial="K" size="xs" class="flex mr-1 place-content-center" cls="positive"></avatar>Karthick Thangaraju
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
      <!-- END: Profile Card -->
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