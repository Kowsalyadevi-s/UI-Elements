<template>
  <Layout class="debug-screens grid sm:grid-cols-12 sm:gap-1">
    <div class="sm:col-span-4 md:col-span-3 lg:col-span-2 border-r">
      <ReportsNavigation />
    </div>
    <div class="sm:col-span-8 md:col-span-9 lg:col-span-10 px-3">
      <div class="flex h-14 justify-between place-items-center">
        <btn-group>
          <btn2 size="xs" variant="dark">All</btn2>
          <btn2 size="xs">Circle</btn2>
          <btn2 size="xs">Polygon</btn2>
        </btn-group>
        <div class="flex space-x-1">
          <Btn2 variant="dark" size="xs">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 mr-1"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 3a1 1 0 011 1v5h5a1 1 0 110 2h-5v5a1 1 0 11-2 0v-5H4a1 1 0 110-2h5V4a1 1 0 011-1z"
                clip-rule="evenodd"
              />
            </svg>
            Create Geofence
          </Btn2>
          <Btn2 size="xs">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 mr-1"
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M4 2a1 1 0 011 1v2.101a7.002 7.002 0 0111.601 2.566 1 1 0 11-1.885.666A5.002 5.002 0 005.999 7H9a1 1 0 010 2H4a1 1 0 01-1-1V3a1 1 0 011-1zm.008 9.057a1 1 0 011.276.61A5.002 5.002 0 0014.001 13H11a1 1 0 110-2h5a1 1 0 011 1v5a1 1 0 11-2 0v-2.101a7.002 7.002 0 01-11.601-2.566 1 1 0 01.61-1.276z"
                clip-rule="evenodd"
              />
            </svg>Refresh
          </Btn2>
          <input type="text" placeholder="Search" />
        </div>
      </div>
      <div class="py-5 space-y-3">
        <Location
          :lat="12.885896904481758"
          :lng="80.09654458608769"
          address="Vandalur, Tamil Nadu 600048"
          :geofence="geofence"
          invalidText="Location varala pa..."
        />
        <Location
          :lat="12.885896904481758"
          :lng="80.09654458608769"
          address="Vandalur, Tamil Nadu 600048"
          :geofence="geofence"
          :showLatLng="false"
          invalidText="Location varala pa..."
        />
        <Location
          :lat="12.885896904481758"
          :lng="80.09654458608769"
          address="Vandalur, Tamil Nadu 600048"
          :geofence="geofence"
          :showAddress="false"
          invalidText="Location varala pa..."
        />
        <Location
          :lat="12.885896904481758"
          :lng="80.09654458608769"
          address="Vandalur, Tamil Nadu 600048"
          invalidText="Location varala pa..."
        />
        <Location
          :lat="12.885896904481758"
          :lng="80.09654458608769"
          invalidText="Location varala pa..."
        />
        <Location :lat="0" :lng="0" invalidText="Location varala pa..." />
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      geofence: {
        geofenceId: "123213123",
        geofenceName: "White Tiger Point",
        geofenceType: "polygon",
      },
    };
  },
};
</script>

<style lang="postcss" scoped>
</style>