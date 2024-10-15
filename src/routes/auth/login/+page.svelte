<script lang="ts">
  let formData = {
    email: '',
    password: ''
  };
  const handleChange = (event: Event) => {
    const target = event.target as HTMLInputElement;
    formData = {
      ...formData,
      [target.name]: target.value
    };
  };

  const handleSubmit = () => {
    console.log(formData);
  };
</script>

<div>
  <h1>Login</h1>
  <form on:submit|preventDefault={handleSubmit}>
    <div>
      <label for="email">Email</label>
      <input
        on:change={handleChange}
        bind:value={formData.email}
        type="email"
        name="email"
        id="email"
      />
    </div>
    <div>
      <label for="password">Password</label>
      <input
        on:change={handleChange}
        bind:value={formData.password}
        type="password"
        name="password"
        id="password"
      />
    </div>
    <button type="submit">Login</button>
  </form>
</div>
