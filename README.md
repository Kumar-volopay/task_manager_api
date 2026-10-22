# Task Manager API

A simple REST API built using Ruby on Rails to manage tasks.

## Features
- Create a task
- View all tasks
- View a single task
- Update a task
- Delete a task
- Validate task data

## Tech Stack
- Ruby
- Ruby on Rails
- PostgreSQL
- RSpec
- RuboCop
- Brakeman
- Bundler Audit

## Setup

1. Clone the repository.
2. Install dependencies:

   ```bash
   bundle install
   ```

3. Start PostgreSQL and Redis using Docker:

   ```bash
   docker compose up -d
   ```

4. Create and prepare the database:

   ```bash
   bundle exec rails db:prepare
   ```

5. Start the Rails server:

   ```bash
   bundle exec rails server
   ```

The API will be available at `http://localhost:3000`.

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/tasks` | Get all tasks |
| GET | `/tasks/:id` | Get a task |
| POST | `/tasks` | Create a task |
| PATCH | `/tasks/:id` | Update a task |
| DELETE | `/tasks/:id` | Delete a task |

## Run Tests

```bash
bundle exec rspec
```

## Code Quality and Security

```bash
bundle exec rubocop
bundle exec brakeman --no-pager
bundle exec bundler-audit check --update
```

## License

For educational and development purposes.
