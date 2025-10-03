<script setup lang="ts">
import type { NavigationMenuItem } from "@nuxt/ui";

const items: NavigationMenuItem[] = [
  {
    label: "Routing",
    icon: "i-lucide-route",
    defaultOpen: true,
    children: [
      { label: "Pages", to: "/routing/pages" },
      { label: "Dynamic Routes", to: "/routing/dynamic-routes" },
      { label: "Nested Routes", to: "/routing/nested-routes" },
      { label: "Middleware", to: "/routing/middleware" },
    ],
  },
  {
    label: "Rendering",
    icon: "i-lucide-server",
    defaultOpen: true,
    children: [
      { label: "SSR (Server-Side Rendering)", to: "/rendering/ssr" },
      { label: "CSR (Client-Side Rendering)", to: "/rendering/csr" },
      { label: "SSG (Static Site Generation)", to: "/rendering/ssg" },
      { label: "ISR (Incremental Static Regeneration)", to: "/rendering/isr" },
    ],
  },
  {
    label: "Data",
    icon: "i-lucide-database",
    defaultOpen: true,
    children: [
      { label: "useFetch()", to: "/data/fetch" },
      { label: "useAsyncData()", to: "/data/async-data" },
      { label: "Server API Routes", to: "/data/server-api-routes" },
      { label: "State (useState)", to: "/data/state" },
    ],
  },
  {
    label: "UI & Composables",
    icon: "i-lucide-components",
    children: [
      { label: "useHead()", to: "/ui-composables/head" },
      { label: "useSeoMeta()", to: "/ui-composables/seo-meta" },
      { label: "Teleport", to: "/ui-composables/teleport" },
      { label: "Suspense", to: "/ui-composables/suspense" },
    ],
  },
  {
    label: "Security",
    icon: "i-lucide-shield-check",
    children: [
      { label: "Runtime Config", to: "/security/runtime-config" },
      { label: "Server Middleware", to: "/security/server-middleware" },
      { label: "Auth", to: "/security/auth" },
    ],
  },
  {
    label: "Modules",
    icon: "i-lucide-package",
    children: [
      { label: "Nuxt UI", to: "/modules/ui" },
      { label: "Nuxt Image", to: "/modules/image" },
      { label: "Nuxt Content", to: "/modules/content" },
      { label: "Third Party Modules", to: "/modules/third-party" },
    ],
  },
];
</script>

<template>
  <UDashboardGroup>
    <UDashboardSidebar collapsible>
      <template #header>
        <UDashboardNavbar
          title="Nuxt.js Dev"
          icon="i-lucide-rocket"
          class="w-full !px-0"
        >
          <template #right>
            <UColorModeButton />
          </template>
        </UDashboardNavbar>
      </template>
      <UNavigationMenu :items="items" orientation="vertical" />
    </UDashboardSidebar>
    <UMain class="w-full">
      <slot />
    </UMain>
  </UDashboardGroup>
</template>
