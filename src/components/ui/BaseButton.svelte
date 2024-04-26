<button>
  <slot />
</button>

<style>
  button {
    font-weight: 700;
    padding: 16px 40px;
    background-color: #1d2130;
    color: #fff;
    border-radius: 12px;
    cursor: pointer;
    transition: background-color ease-out 0.5s;

    &:hover {
      background-color: #313852;
    }
  }
</style>
