<script setup lang="ts">
import type { NavigationMenuItem } from "@nuxt/ui";

const items: NavigationMenuItem[] = [
  {
    label: "Routing",
    icon: "i-lucide-route",
    defaultOpen: true,
    children: [
      { label: "Pages" },
      { label: "Dynamic Routes" },
      { label: "Nested Routes" },
      { label: "Middleware" },
    ],
  },
  {
    label: "Rendering",
    icon: "i-lucide-server",
    defaultOpen: true,
    children: [
      { label: "SSR (Server-Side Rendering)" },
      { label: "CSR (Client-Side Rendering)" },
      { label: "SSG (Static Site Generation)" },
      { label: "ISR (Incremental Static Regeneration)" },
    ],
  },
  {
    label: "Data",
    icon: "i-lucide-database",
    defaultOpen: true,
    children: [
      { label: "useFetch()" },
      { label: "useAsyncData()" },
      { label: "Server API Routes" },
      { label: "State (useState)" },
    ],
  },
  {
    label: "UI & Composables",
    icon: "i-lucide-components",
    children: [
      { label: "useHead()" },
      { label: "useSeoMeta()" },
      { label: "Teleport" },
      { label: "Suspense" },
    ],
  },
  {
    label: "Security",
    icon: "i-lucide-shield-check",
    children: [
      { label: "Runtime Config" },
      { label: "Server Middleware" },
      { label: "Auth" },
    ],
  },
  {
    label: "Modules",
    icon: "i-lucide-package",
    children: [
      { label: "Nuxt UI" },
      { label: "Nuxt Image" },
      { label: "Nuxt Content" },
      { label: "Third Party Modules" },
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
    <UMain><slot /></UMain>
  </UDashboardGroup>
</template>
