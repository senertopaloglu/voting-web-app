# voting-web-app

A beautiful, scalable real-time voting app made using Next.js and serverless Redis DB hosted at [Upstash](upstash.com)

User's can create "rooms" to vote/provide feedback on topics, and other users can simply enter the same topic to join the discussion. 

The application has been designed for maximum scalability, many "rooms" can exist at the same time and multiple users can interact with the application simultaneously. Naturally, Redis was a sound choice to meet such requirements.

### How to run
#### Prerequistes
Please ensure you have NodeJS, npm and TypeScript installed.

In order to use Upstash Redis hosting, please create an Upstash account, then proceed to create a new (free) database instance [here](https://console.upstash.com/redis) - billing information is not required.

#### Instructions

1. `git clone` this repository
2. `cd` into repository on machine
3. `cd` into `/server`:
    1. `npm install` to install all dependencies for the voting server.
    2. `npm run dev` to compile and start the voting server.
4. open another terminal window and `cd` into `/client`:
    1. `npm install` to install all dependencies for the voting client.
    2. `npm run dev` to compile and start the voting client.
    3. Please navigate to `http://localhost:3000` in the browser (localhost connection can be configured in `\server\index.ts`)
