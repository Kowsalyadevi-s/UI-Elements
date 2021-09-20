<template>
  <div>
    <header class="flex flex-justify between bg-gray-100 p-4">
      <div>
      <nav>
        <ul class="flex">
          <li class="mr-6">
            <a class=" hover:text-blue-800" href="#">Dashboard</a>
          </li>
          <li class="mr-6">
            <a class=" hover:text-blue-800" href="#">Tanks</a>
          </li>
          <li class="mr-6">
            <a class=" hover:text-blue-800" href="#">Mapping</a>
          </li>
          
        </ul>
      </nav>
      </div>

<div>
      <nav class="inline-block">
        <ul class="flex">
          <li class="mr-6">
            <a class="text-blue-500 hover:text-blue-800" href="#">Dashboard</a>
          </li>
          <li class="mr-6">
            <a class="text-blue-500 hover:text-blue-800" href="#">Tanks</a>
          </li>
        </ul>
      </nav>
</div>
    </header>

    <div class="flex justify-between w-full ">
      <div>
        <nav class="rounded  p-4">
          <ol class="flex text-grey-dark">
            <li><span class="mx-2">Account:Fuji/</span></li>
            <li><a href="#" class="text-blue font-bold">Tanks</a></li>
            <li><span class="mx-2">/</span></li>
            <li>FFMU 2020777</li>
          </ol>
        </nav>
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
        <btn2 variant="primary">Send Command</btn2>
        <dropdown label="Actions">
          <div class="py-1">
            <dropdown-item>Option 1</dropdown-item>
            <dropdown-item>Option 1</dropdown-item>
          </div>
        </dropdown>

        <div class="relative inline-block">
          <span class="absolute inset-y-0 flex items-center pl-2 text-gray-400">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
              />
            </svg>
          </span>
          <input
            type="text"
            class="
              w-64
              h-9
              px-10
              rounded
              focus:outline-none
              focus:ring-2 focus:ring-primary
              focus:border-transparent
              hover:bg-gray-50
              hover:border-gray-400
              hover:text-gray-900
              border-opacity-50 border border-gray-
            "
            placeholder="Search Tank Name"
          />
        </div>
      </div>
    </div>

    <div class="grid grid-cols-3 gap-4 w-full p-4 bg-gray-100">
      <div class="grid grid-rows-3 gap-2">
        <div>
          <card class="space-y-2 p-2">
                <div>
                  <p>Tank Details</p>
                </div>
                <div>
                  <p>Tank name</p>
                  <h6>FFMU2027666</h6>
                </div>

                <div class="space-y-2">
                  <p>Location</p>
                  <span class="inline-flex space-x-2">
                    <span
                      ><badge class="positive filled flex-1">IN</badge></span
                    >
                    <span
                      ><h6 class="uppercase flex-1">fuji - mesa az</h6></span
                    >
                  </span>
                  <p class="text-xs text-gray-400">
                    (33.2980184555, -111.5935742855)
                  </p>
                  <a href="#">Poll location</a>
                </div>
          </card>
        </div>

        <!-- <div>
          <card class="">
            <div class="grid grid-cols-2 gap-2">

              <div class="space-y-2 p-2">
                <div>
                  <p>Tank Properties</p>
                </div>
                <div>
                  <p>Liquid Type</p>
                  <h6>PGMEA</h6>
                </div>

                <div class="space-y-2 p-2">
                  <div>
                    <p>Tank Properties</p>
                  </div>
                  <div>
                    <p>Liquid Type</p>
                    <h6>PGMEA</h6>
                  </div>
                </div>
              </div>

                <div>
              <div class="space-y-2 p-2">
                <div>
                  <p>Tank Properties</p>
                </div>
                <div>
                  <p>Liquid Type</p>
                  <h6>PGMEA</h6>
                </div>

                <div class="space-y-2 p-2">
                  <div>
                    <p>Tank Properties</p>
                  </div>
                  <div>
                    <p>Liquid Type</p>
                    <h6>PGMEA</h6>
                  </div>
                </div>
              </div>



              </div>
            </div>
          </card>
        </div>

        <div>
          <card class="">
            <div class="grid grid-cols-2 gap-2">

              <div>
              <div class="space-y-2 p-2">
                <div>
                  <p>Tank Properties</p>
                </div>
                <div>
                  <p>Liquid Type</p>
                  <h6>PGMEA</h6>
                </div>

                <div class="space-y-2 p-2">
                  <div>
                    <p>Tank Properties</p>
                  </div>
                  <div>
                    <p>Liquid Type</p>
                    <h6>PGMEA</h6>
                  </div>
                </div>
              </div>

                <div>
              <div class="space-y-2 p-2">
                <div>
                  <p>Tank Properties</p>
                </div>
                <div>
                  <p>Liquid Type</p>
                  <h6>PGMEA</h6>
                </div>

                <div class="space-y-2 p-2">
                  <div>
                    <p>Tank Properties</p>
                  </div>
                  <div>
                    <p>Liquid Type</p>
                    <h6>PGMEA</h6>
                  </div>
                </div>
              </div>

              </div>


              </div>
            </div>
          </card>
        </div> -->
      </div>

      <div class="col-span-2 bg-green-200">
        <h1>Tank status</h1>
      </div>
    </div>
  </div>
</template>






