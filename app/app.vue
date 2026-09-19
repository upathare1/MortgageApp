<script setup lang="ts">
useHead({
  htmlAttrs: { lang: 'en' },
  link: [{ rel: 'icon', type: 'image/svg+xml', href: '/favicon.svg' }]
})
useSeoMeta({
  title: 'MortgageApp | Buy vs. rent',
  description: 'Compare buying a home with renting and investing over the same time horizon.'
})
</script>

<template>
  <UApp>
    <div class="flex min-h-screen flex-col">
      <UHeader>
        <template #left>
          <NuxtLink
            to="/"
            class="flex items-center gap-2 font-semibold text-highlighted"
          >
            <UIcon
              name="i-lucide-house"
              class="size-5 text-primary"
            />
            MortgageApp
          </NuxtLink>
        </template>
        <template #right>
          <UColorModeButton />
        </template>
      </UHeader>
      <main class="flex-1">
        <NuxtPage />
      </main>
      <footer class="shrink-0 border-t border-default py-3">
        <UContainer>
          <p class="text-center text-sm text-muted">
            Copyright &copy; {{ new Date().getFullYear() }} Upamanyu Pathare. Licensed under the GNU Affero General Public License v3.0.
          </p>
          <p class="mx-auto mt-1 max-w-4xl text-center text-xs leading-5 text-muted">
            This calculator provides estimates for informational purposes only. Results are not guaranteed to be accurate or complete and should not be relied upon as financial, tax, or legal advice. Please consult a qualified professional before making financial decisions.
          </p>
        </UContainer>
      </footer>
    </div>
  </UApp>
</template>
