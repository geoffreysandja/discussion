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
  * Make sure to create a Github Application (This app uses OAuth Login with Github) and modify config/config.exs

  ```elixir
  config :ueberauth, Ueberauth,
  providers: [
    github: { Ueberauth.Strategy.Github, [default_scope: "user,user:email,public_repo"] }
  ]
config :ueberauth, Ueberauth.Strategy.Github.OAuth,
  client_id: "",
  client_secret: ""
  
  ```
  
To start your Phoenix app:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.create && mix ecto.migrate`
  * Install Node.js dependencies with `npm install`
  * Start Phoenix endpoint with `mix phoenix.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.
