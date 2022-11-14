<template>
  <div>
    <p style="border: 1px solid; padding: 0.5rem">
      <slot />
    </p>
    <hr />
    <slot name="namedSlot" />
  </div>
</template>
