<template>
  <form>
    <div class="help">
      <slot name="help"></slot>
    </div>
    <div class="field">
      <slot name="field"></slot>
    </div>
    <div class="button">
      <slot name="button"></slot>
    </div>
    <slot></slot>
  </form>
</template>
