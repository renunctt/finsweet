<script>
  import BaseButton from './BaseButton.svelte'
</script>

<div class="form">
  <input type="email" placeholder="Enter Your Email" />
  <BaseButton>Get Free trial</BaseButton>
</div>

<style>
  .form {
    width: 576px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 48px;
    padding: 8px;
    background-color: #fff;
    border-radius: 12px;
  }

  input {
    width: 330px;
    font-size: 18px;
    padding: 4px 20px;
  }
</style>
