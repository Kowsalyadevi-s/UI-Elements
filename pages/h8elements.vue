<template>
  <Layout class="container p-5">
    <div>
      <Heading>
        <h2>H8UI Element Collections</h2>
        <p
          class="muted"
        >Base Web offers a robust suite of components out of the box. These include complex, ready-to-use components such as Datepicker and low-level composable primitives, such as Layer.</p>
      </Heading>
      <div class="flex flex-col space-y-6 p-4">
        <div class>
          <Heading>
            <h4>Buttons</h4>
            <p
              class="muted"
            >Buttons provide cues for actions and events. These fundamental components allow users to process actions or navigate an experience.</p>
          </Heading>
          <div class="flex flex-col space-y-4">
            <div class="space-y-2">
              <h6>Variations</h6>
              <div class="space-x-1">
                <btn2 variant="null">Welcome Button</btn2>
                <btn2>Welcome Button</btn2>
                <btn2 variant="primary">Welcome Button</btn2>
                <btn2 variant="dark">Welcome Button</btn2>
                <btn2 variant="positive">Welcome Button</btn2>
                <btn2 variant="negative">Welcome Button</btn2>
              </div>
            </div>
            <div class="space-y-2">
              <h6>Shape</h6>
              <div class="space-x-1">
                <btn2>Welcome Button</btn2>
                <btn2 shape="rounded">Welcome Button</btn2>
                <btn2 shape="square">Welcome Button</btn2>
              </div>
            </div>
            <div class="space-y-2">
              <h6>Disabled</h6>
              <div class="space-x-1 flex">
                <btn2 disabled variant="null">Welcome Button</btn2>
                <btn2 disabled>Welcome Button</btn2>
                <btn2 disabled variant="primary">Welcome Button</btn2>
                <btn2 disabled variant="dark">Welcome Button</btn2>
                <btn2 disabledvariant="positive">Welcome Button</btn2>
                <btn2 disabled variant="negative">Welcome Button</btn2>
              </div>
            </div>
            <div class="space-y-2">
              <h6>Size</h6>
              <div class="space-x-1 flex place-items-end">
                <btn2 variant="primary" size="xs">Welcome Button</btn2>
                <btn2 variant="primary" size="sm">Welcome Button</btn2>
                <btn2 variant="primary">Welcome Button</btn2>
                <btn2 variant="primary" size="lg">Welcome Button</btn2>
                <btn2 variant="primary" size="xl">Welcome Button</btn2>
              </div>
            </div>
            <div class="space-y-2">
              <h6>Icon + Label</h6>
              <div class="space-x-1 flex place-items-end">
                <btn2 variant="primary" size="xs">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-4 w-4"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M12 6v6m0 0v6m0-6h6m-6 0H6"
                    />
                  </svg>
                  Welcome Button
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-4 w-4"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M13 7l5 5m0 0l-5 5m5-5H6"
                    />
                  </svg>
                </btn2>
                <btn2 variant="primary" size="sm">
                  <icon />Welcome Button
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-4 w-4"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M13 7l5 5m0 0l-5 5m5-5H6"
                    />
                  </svg>
                </btn2>
                <btn2 variant="primary">
                  <icon />Welcome Button
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-4 w-4"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M13 7l5 5m0 0l-5 5m5-5H6"
                    />
                  </svg>
                </btn2>
                <btn2 variant="primary" size="lg">
                  <icon />Welcome Button
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-4 w-4"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M13 7l5 5m0 0l-5 5m5-5H6"
                    />
                  </svg>
                </btn2>
                <btn2 variant="primary" size="xl">
                  <icon />Welcome Button
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-4 w-4"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M13 7l5 5m0 0l-5 5m5-5H6"
                    />
                  </svg>
                </btn2>
              </div>
            </div>

            <div class="space-y-2">
              <h6>Outlined</h6>
              <div class="space-x-1">
                <btn2 variant="primary" outlined>Welcome Button</btn2>
              </div>
            </div>
          </div>
        </div>
        <div>
          <Heading>
            <h4>Button Groups</h4>
            <p
              class="muted"
            >Buttons provide cues for actions and events. These fundamental components allow users to process actions or navigate an experience.</p>
          </Heading>
          <div class="space-y-2">
            <h6>Outlined</h6>
            <div class="space-x-1">
              <div class="flex flex-col space-y-2">
                <btn-group>
                  <btn2 size="xl">Button 1</btn2>
                  <btn2 class="dark" size="xl">Button 2</btn2>
                  <btn2 size="xl">Button 3</btn2>
                  <btn2 size="xl">Button 4</btn2>
                </btn-group>
                <btn-group>
                  <btn2 variant="dark" size="lg">Button 1</btn2>
                  <btn2 size="lg">Button 2</btn2>
                  <btn2 size="lg">Button 3</btn2>
                  <btn2 size="lg">Button 4</btn2>
                </btn-group>
                <btn-group>
                  <btn2 variant="dark">Button 1</btn2>
                  <btn2>Button 2</btn2>
                  <btn2>Button 3</btn2>
                  <btn2>Button 4</btn2>
                </btn-group>
                <btn-group>
                  <btn2 variant="dark" size="sm">Button 1</btn2>
                  <btn2 size="sm">Button 2</btn2>
                  <btn2 size="sm">Button 3</btn2>
                  <btn2 size="sm">Button 4</btn2>
                </btn-group>
                <btn-group>
                  <btn2 variant="dark" size="xs">Button 1</btn2>
                  <btn2 size="xs">Button 2</btn2>
                  <btn2 size="xs">Button 3</btn2>
                  <btn2 size="xs">Button 4</btn2>
                </btn-group>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import BtnGroup from "../components/elements/BtnGroup.vue";
export default {
  components: { BtnGroup },
};
</script>

<style lang="postcss" scoped>
</style>