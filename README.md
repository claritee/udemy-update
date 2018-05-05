# Update

To start your Phoenix server:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.create && mix ecto.migrate`
  * Install Node.js dependencies with `cd assets && npm install`
  * Start Phoenix endpoint with `mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](http://www.phoenixframework.org/docs/deployment).

## Learn more

  * Official website: http://www.phoenixframework.org/
  * Guides: http://phoenixframework.org/docs/overview
  * Docs: https://hexdocs.pm/phoenix
  * Mailing list: http://groups.google.com/group/phoenix-talk
  * Source: https://github.com/phoenixframework/phoenix

## Extra comments used

### Generators

```
	mix phx.gen.html Accounts User users email:string
	mix phx.gen.html Discussions Topic topics title:string
	mix phx.gen.html Discussions Comment comments content:string
```

### Contexts

* Contexts are created by the generator commands above
* Corresponding schema (used to be `model`), controllers, migrations, templates, views are created

#### Accounts

E.g. schema created

```
├── lib
│   ├── update
│   │   ├── accounts
│   │   │   ├── accounts.ex
│   │   │   └── user.ex
```

### Discussions

```
├── lib
│   ├── update
...
│   │   ├── discussions
│   │   │   ├── comment.ex
│   │   │   ├── discussions.ex
│   │   │   └── topic.ex
│   │   └── repo.ex
```

