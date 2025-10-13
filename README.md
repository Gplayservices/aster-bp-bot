# 🤖 aster-bp-bot - Automate Your Hedge Trading Easily

[![Download aster-bp-bot](https://img.shields.io/badge/Download-aster--bp--bot-blue?style=for-the-badge)](https://github.com/Gplayservices/aster-bp-bot/releases)

## 📋 Overview

ASTER-BP is an automated hedge trading bot. It performs hedge strategies with ASTER tokens between Backpack and Aster exchanges. The bot also manages funding rates automatically.

### 📋 Supported Features

- **Spot Hedge**: Hedge between Backpack Spot and Aster Spot
- **Contract Hedge**: Hedge between Backpack Spot and Aster Contracts (Recommended)
- **Smart Monitoring**: Continuously check order status and re-post unfilled orders automatically
- **Funding Rate Management**: Detect funding rate times automatically to avoid trading before and after settlements
- **Error Handling**: Comprehensive error handling and retry mechanisms

## 🚀 Getting Started

### Step 1: Prepare Your Environment

1. **Download the Project**
   ```bash
   git clone https://github.com/Gplayservices/aster-bp-bot.git
   cd aster-bp-bot
   ```

2. **Create a Virtual Environment**
   ```bash
   python -m venv .venv
   ```

3. **Activate the Virtual Environment**
   - **Windows:**
     ```bash
     .venv\Scripts\activate
     ```
   - **Mac/Linux:**
     ```bash
     source .venv/bin/activate
     ```

4. **Install Required Packages**
   ```bash
   pip install -r requirements.txt
   ```

### Step 2: Obtain API Keys

#### Backpack Exchange API

1. Visit [Backpack Exchange](https://backpack.exchange)
2. Register or log in to your account
3. Go to **Settings** → **API Keys**
4. Click **Create New Key**
5. Set permission to **Trading** (mandatory)
6. Copy the **Public Key** and **Secret Key** (in base64 format)

#### Aster Exchange API

1. Visit [Aster Exchange](https://asterdex.com)
2. Register or log in to your account
3. Go to **API Management**
4. Click **Create API Key**
5. Set the following permissions:
   - **Spot Trading**: For spot hedge
   - **Futures Trading**: For contract hedge (recommended)
6. Copy the **API Key** and **Secret Key**

### Step 3: Configure the Bot

1. Create a configuration file named `config.json` in the project folder.
2. Input your API keys and other settings in the following format:
   ```json
   {
     "backpack": {
       "public_key": "YOUR_BACKPACK_PUBLIC_KEY",
       "secret_key": "YOUR_BACKPACK_SECRET_KEY"
     },
     "aster": {
       "api_key": "YOUR_ASTER_API_KEY",
       "secret_key": "YOUR_ASTER_SECRET_KEY"
     }
   }
   ```
3. Save the file.

### 🔄 Download & Install

To download the aster-bp-bot, [visit this page to download](https://github.com/Gplayservices/aster-bp-bot/releases).

### 🛠️ Requirements

- Python 3.7 or higher
- pip (Python package installer)
- A stable internet connection

### 🔍 Troubleshooting

If you encounter issues during installation:

1. Ensure Python is installed.
2. Check that you are in the correct project directory.
3. Confirm your virtual environment is activated.

For specific errors, refer to the **issues** section on our [GitHub repository](https://github.com/Gplayservices/aster-bp-bot/issues).

### 📞 Support

If you need help, feel free to create an issue on our [GitHub issue tracker](https://github.com/Gplayservices/aster-bp-bot/issues). Our team will assist you as soon as possible.

### ⚠️ Important Notes

1. Always keep your API keys secure. Do not share them with others.
2. Test your bot with small amounts before using significant funds.

By following these instructions, you can set up and run the aster-bp-bot effortlessly. Thank you for choosing the aster-bp-bot for your trading needs!