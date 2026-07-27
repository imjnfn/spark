```md
# spark ai

spark ai is a lightweight desktop application that automatically installs and manages a chrome extension for ai-powered screen text capture.

the application is fully self-contained. after running the installer, no manual extension loading, developer mode, or additional setup is required.

## features

- automatic installation
- automatic chrome extension setup
- screen text capture
- ai-powered responses
- fast and lightweight
- local configuration storage
- no external backend
- automatic gemini api key rotation
- automatic fallback providers

## ai providers

spark ai uses **google gemini** as its primary provider.

the selected gemini model is limited to approximately **6 requests per minute per api key**. to reduce this limitation, spark ai supports configuring up to **three gemini api keys** and automatically rotates between them.

if every configured gemini key is rate-limited or unavailable, spark ai automatically switches to one of the configured backup providers.

supported backup providers:

- openrouter
- groq
- openai

these providers are only used when gemini cannot process a request.

## installation

1. download the latest `spark ai setup.exe` from the releases page.
2. run the installer.
3. launch spark ai.
4. enter at least one gemini api key.
5. optionally configure backup providers.

that's it.

## configuration

spark ai stores all settings locally on your device.

supported configuration includes:

- up to three gemini api keys
- openrouter api key
- groq api key
- openai api key
- ai model selection
- extension preferences

api keys are only sent directly to the provider they belong to when making requests.

## privacy

spark ai does not use a backend server.

all requests are sent directly from your device to the configured ai provider. configuration and api keys remain stored locally.

## disclaimer

this project is provided as-is without any warranty or guarantee of support.
```
