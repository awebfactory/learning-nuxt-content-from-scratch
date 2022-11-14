<template>
  <aside>
    <h2>Nested component</h2>
    <ContentSlot :use="$slots.default" unwrap="p" />
  </aside>
</template>
