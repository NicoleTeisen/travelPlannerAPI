# Plann.er - Back end

Back end created to be the API that will send data to a travel and activity planner.

## Technologies Used

- [Fastify](https://www.fastify.io/) - Fast and low-overhead web framework
- [Prisma](https://www.prisma.io/) - Modern ORM
- [Zod](https://github.com/colinhacks/zod) - Type schema validation
- [Nodemailer](https://nodemailer.com/about/) - Email sending
- [Day.js](https://day.js.org/) - Date manipulation
- [TypeScript](https://www.typescriptlang.org/) - JavaScript superset that adds static types
- [@fastify/cors](https://github.com/fastify/fastify-cors) - Fastify plugin to enable CORS

## Installation

To install the project dependencies, run the following command:

```bash
npm install
```

## Environment Configuration

Create a `.env` file at the root of the project and add the following environment variables:

```env
DATABASE_URL="file:./dev.db"
API_BASE_URL="http://localhost:3333"
WEB_BASE_URL="http://localhost:3000"
PORT=3333
```

## How to Run

To start the server, use the following command:

```bash
npm run dev
```

The server will be running at `http://localhost:3333`.

## Routes

### `POST /trips`

Creates a new trip.

### `POST /trips/confirm`

Confirms a trip.

### `POST /trips/participants/confirm`

Confirms trip participants.

### `POST /activities`

Creates a new activity.

### `GET /activities`

Returns the list of activities.

### `POST /links`

Creates a new link.

### `GET /links`

Returns the list of links.

### `GET /participants`

Returns the list of participants.

### `POST /invites`

Creates a new invite.

### `PUT /trips/:id`

Updates a trip.

### `GET /trips/:id`

Returns the details of a trip.

### `GET /participants/:id`

Returns the details of a participant.

## Contribution

If you want to contribute to the project, follow the steps below:

1. Fork the project
2. Create a branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Open a Pull Request
