# Clubs Trump API Proxy

This is a serverless proxy that allows the Clubs Trump scorekeeper to call the Anthropic API without CORS issues.

## Setup on Vercel

1. Push these files to a new GitHub repository
2. Import the repository in Vercel
3. Add environment variable: `ANTHROPIC_API_KEY` with your API key
4. Deploy!

## Environment Variables

- `ANTHROPIC_API_KEY`: Your Anthropic API key (sk-ant-...)

## Endpoint

POST `/api/generate-poem`

Request body:
```json
{
  "prompt": "Your prompt here"
}
```

Response:
```json
{
  "poem": "Generated poem text"
}
```
