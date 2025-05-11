---

<p align="center">
  <strong>Boost your productivity with Animix Bot – your friendly automation tool that handles key tasks with ease!</strong>
</p>

<p align="center">
  <a href="https://github.com/Jhinkz018/animix">
    <img src="https://img.shields.io/badge/build-passed-brightgreen" alt="Build Status" />
  </a>
  <a href="https://discord.gg/WfgGg8n9">
    <img src="https://img.shields.io/badge/Discord-Join%20Server-5865F2?logo=discord&style=flat" alt="Discord Server" />
  </a>
</p>


---

## 🚀 About the Bot

Animix Bot is your automation buddy designed to simplify daily operations. This bot takes over repetitive tasks so you can focus on what really matters. With Animix Bot, you get:

- **🎰 Auto Gacha:**  
  Automatically perform gacha pulls to maximize your rewards.
- **🏆 Auto Achievements:**  
  Claim achievements automatically to keep your bonus collection growing.
- **🧬 Auto DNA Mixing:**  
  Use a custom mix system (configured via a `dna.json` file) to automatically mix DNA while avoiding combinations with pets that have a star rating greater than 4.
- **🗺️ Auto Missions & Quests:**  
  Complete missions and quests automatically without manual intervention.
- **🎫 Auto Claim Pass:**  
  Claim pass rewards automatically for maximum benefit.
- **⚔️ Auto PvP & Defense Setup:**  
  Engage in PvP battles automatically and configure your defense team for better performance.
- **⏫ Pet Upgrade System:**  
  Automatically upgrade pets with 4 stars or higher to boost your gameplay.
- **Multi Account Support 👥:**  
  Manage multiple accounts effortlessly with built-in multi account support.
- **Thread System 🧵:**  
  Run tasks concurrently with configurable threading options to improve overall performance and speed.
- **Configurable Delays ⏱️:**  
  Fine-tune delays between account switches and loop iterations to match your specific workflow needs.
- **Support Proxy 🔌:**  
  Use HTTP/HTTPS proxies to enhance your multi-account setups.

Animix Bot is built with flexibility and efficiency in mind – it's here to help you automate your operations and boost your productivity!

---

## 🌟 Version Updates

**Current Version: v1.5.0**

### v1.5.0 - Latest Update

- Adjusted to match Animix server’s latest header updates
- Fixed external server for mix data logging following the main GitHub account suspension incident

---

## 📝 Register

Before you start using Animix Bot, make sure to register your account.  
Click the link below to get started:

[🔗 Register for Animix Bot](https://t.me/animix_game_bot?startapp=3lsLj56QYJx6)

---

## ⚙️ Configuration

### Main Bot Configuration (`config.json`)

```json
{
  "gacha": true,
  "achievements": true,
  "mix": true,
  "mission": true,
  "quest": true,
  "claim_pass": true,
  "pvp": true,
  "proxy": false,
  "thread": 1,
  "delay_loop": 3000,
  "delay_account_switch": 10,
  "pet_mix": [
    [122, 125],
    [125, 121],
    [124, 125],
    [118, 116],
    [119, 115],
    [120, 113]
  ],
  "defens_type": "armor",
  "defens_id": [],
  "attack_type": "damage",
  "attack_id": []
}
```

| **Setting**            | **Description**                                                      | **Default Value** |
| ---------------------- | -------------------------------------------------------------------- | ----------------- |
| `gacha`                | Enable automatic gacha pulls.                                        | `true`            |
| `achievements`         | Automatically claim achievements.                                    | `true`            |
| `mix`                  | Automate DNA mixing.                                                 | `true`            |
| `mission`              | Complete missions automatically.                                     | `true`            |
| `quest`                | Execute quests without manual intervention.                          | `true`            |
| `claim_pass`           | Automatically claim pass rewards.                                    | `true`            |
| `pvp`                  | Enable automatic PvP battles.                                        | `true`            |
| `proxy`                | Enable proxy usage for multi-account setups.                         | `false`           |
| `thread`               | Number of threads to run tasks concurrently.                         | `1`               |
| `delay_loop`           | Delay (in seconds) before the next loop begins.                      | `3000`            |
| `delay_account_switch` | Delay (in seconds) between switching accounts.                       | `10`              |
| `pet_mix`              | Custom configuration for pet mixing.                                 | See above         |
| `defens_type`          | Attribute for defense selection (e.g., armor, hp, speed, damage).    | `"armor"`         |
| `defens_id`            | Specific pet IDs for defense configuration.                          | `[]`              |
| `attack_type`          | Attribute for PvP attack selection (e.g., armor, hp, speed, damage). | `"damage"`        |
| `attack_id`            | Specific pet IDs for PvP attack configuration.                       | `[]`              |

---

## 📅 Requirements

- **Minimum Python Version:** `Python 3.9+`
- **Required Libraries:**
  - colorama
  - requests
  - fake-useragent
  - brotli
  - chardet
  - urllib3

These are installed automatically when running:

```bash
pip install -r requirements.txt
```

---

## 📅 Installation Steps

### Main Bot Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Jhinkz018/animix.git
   ```

2. **Navigate to the Project Folder**

   ```bash
   cd animix-bot
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Configure Your Query**

   Create a file named `query.txt` and add your query data.

5. **Set Up Proxy (Optional)**  
   To use a proxy, create a `proxy.txt` file and add proxies in the format:

   ```
   http://username:password@ip:port
   ```

   _Only HTTP and HTTPS proxies are supported._

6. **Run Bot**

   ```bash
   python main.py
   ```

---

### 🔹 Want Free Proxies?

You can obtain free proxies from [Webshare.io](https://www.webshare.io/).

---

## 📂 Project Structure

```
Animix-bot/
├── config.json                 # Main configuration file for the bot
├── query.txt                   # Contains query data to be processed
├── proxy.txt                   # (Optional) Proxy list (HTTP/HTTPS) to use for multi-account support
├── main.py                     # Main Python script (entry point of the bot)
├── requirements.txt            # Python dependencies required to run the bot
├── LICENSE                     # License for the project
└── README.md                   # Documentation and feature list
```

---

## 🛠️ Contributing

This project is developed by **Livexords**.  
If you have ideas, questions, or want to contribute, please join our Discord server for discussions and updates.  
For contribution guidelines, please consider:

- **Code Style:** Follow standard Python coding conventions.
- **Pull Requests:** Test your changes before submitting a PR.
- **Feature Requests & Bugs:** Report and discuss via our Discord server.

<div align="center">
  <a href="https://discord.gg/WfgGg8n9" target="_blank">
    <img src="https://img.shields.io/badge/Join-Discord%20Server-5865F2?logo=discord&style=for-the-badge" height="25" alt="Discord Server" />
  </a>
</div>

---

## 📖 License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for more details.

---

## 🔍 Usage Example

After installation and configuration, simply run:

```bash
python main.py
```

You should see output indicating the bot has started its operations. For further instructions or troubleshooting, please check our Telegram group or open an issue in the repository.

---

## 📣 Community & Support

For support, updates, and feature requests, join our Discord server.  
This is the central hub for all discussions related to Animix Bot, including roadmap ideas and bug fixes.

---
