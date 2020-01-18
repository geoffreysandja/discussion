# Discuss
This a web application built on Elixir/Phoenix(1.2)

**Make sure to download the Phoenix 1.2 version**

Before running this Phoenix app:
  * Modify the config/dev.exs

  ```elixir
config :discuss, Discuss.Repo,
  adapter: Ecto.Adapters.Postgres,
  username: "",
  password: "",
  database: "",
  hostname: "",
  port: 5432,
  pool_size: 10
  
  ```
  
To start your Phoenix app:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.create && mix ecto.migrate`
  * Install Node.js dependencies with `npm install`
  * Start Phoenix endpoint with `mix phoenix.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.
