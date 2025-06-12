# krypto-botpython-dotenv
krakenex
pandas
ta
KRAKEN_API_KEY=YOUR_KRAKEN_API_KEY
KRAKEN_API_SECRET=YOUR_KRAKEN_API_SECRET
services:
  - type: worker
    name: kraken-bot
    runtime: python
    repo: https://github.com/Golisss/kraken-bot
    branch: main
    buildCommand: pip install -r requirements.txt
    startCommand: python main.py
    envVars:
      - key: KRAKEN_API_KEY
      - key: KRAKEN_API_SECRET
