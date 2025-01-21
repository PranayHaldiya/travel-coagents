# CoAgents Travel

This example contains a Travel Planner application with search capabilities using CoAgents.

[![Watch the video]](https://www.youtube.com/watch?v=9v3kXiOY3vg)

### India Travel Destinations
![India snap](https://github.com/PranayHaldiya/travel-coagents/blob/main/ui/app/Screenshot%202025-01-21%20193102.png)

### Adding India Travel Destinations
![Adding trips snap](https://github.com/PranayHaldiya/travel-coagents/blob/main/ui/app/Screenshot%202025-01-21%20193130.png)

### Vacation in Paris
![Paris snap](https://github.com/PranayHaldiya/travel-coagents/blob/main/ui/app/Screenshot%202025-01-21%20193209.png)

### Business Trip NYC
![NYC snap](https://github.com/PranayHaldiya/travel-coagents/blob/main/ui/app/Screenshot%202025-01-21%20193343.png)

**These instructions assume you are in the `coagents-travel/` directory**

## Running the Agent

This agent is already hosted in LangGraph Platform. However, if you'd like to run it
yourself first, install the dependencies:

```sh
cd agent
poetry install
```

Then, create a `.env` file inside `./agent` with the following:

```
OPENAI_API_KEY=...
GOOGLE_MAPS_API_KEY=...
```

IMPORTANT:
Make sure the OpenAI API Key you provide, supports gpt-4o.

Then, run the demo:

```sh
poetry run demo
```

## Running the UI

First, install the dependencies:

```sh
cd ./ui
pnpm i
```

Then, create a `.env` file inside `./ui` with the following:

```
OPENAI_API_KEY=...
NEXT_PUBLIC_CPK_PUBLIC_API_KEY=...
```

If you need a CopilotKit API key, you can get one [here](https://cloud.copilotkit.ai)

Then, run the Next.js project:

```sh
pnpm run dev
```

## Usage

Navigate to [http://localhost:3000](http://localhost:3000).

# LangGraph Studio

Run LangGraph studio, then load the `./agent` folder into it.

Make sure to create the `.env` files mentioned above first!

# Troubleshooting

A few things to try if you are running into trouble:

1. Make sure there is no other local application server running on the 8000 port.
2. Under `/agent/travel/demo.py`, change `0.0.0.0` to `127.0.0.1` or to `localhost`
