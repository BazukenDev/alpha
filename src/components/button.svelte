<script>
  export let className;
</script>

<button class="button {className}">
  <slot />
</button>

<style lang="scss">
  button {
    display: flex;
    justify-content: center;
    align-items: center;
    border: none;
    background: none;
    border-radius: 15px;
    color: var(--color-stroke);
    width: 40px;
    height: 40px;

    &.primary {
      background-color: var(--color-primary);
    }
  }
</style>
