# LinkLook

A lightweight utility that hosts a **hyper-realistic Zoom Meeting Waiting Room page** and generates a shareable URL using Cloudflare Tunnel. Designed for authorized security awareness demonstrations, user-experience research, and controlled testing environments.

---

## Overview

**LinkLook** creates a realistic Zoom-style waiting room page and exposes it securely through a temporary public URL. The generated link can be shared with test participants for approved demonstrations and research activities.

### Features

* Hyper-realistic Zoom Meeting Waiting Room interface
* Automatic public link generation using Cloudflare Tunnel
* Lightweight PHP-based hosting
* Works on Linux distributions and Termux
* Simple setup and cleanup process
* Automatic logging and file management

---

## Supported Platforms

* Kali Linux
* Ubuntu
* Debian
* Parrot Security OS
* Arch Linux
* Termux
* Other Linux-based distributions

---

## Requirements

Install the required packages:

```bash
sudo apt update
sudo apt install -y php wget unzip git
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/<your-username>/LinkLook.git
```

Navigate to the project directory:

```bash
cd LinkLook
```

Grant execution permissions:

```bash
chmod +x linklook.sh
chmod +x cleanup.sh
```

Run LinkLook:

```bash
bash linklook.sh
```

---

## Usage

### Step 1 – Start LinkLook

```bash
bash linklook.sh
```

### Step 2 – Copy Generated Link

After startup, LinkLook will generate a public Cloudflare Tunnel URL similar to:

```text
https://example.trycloudflare.com
```

Copy the generated link.

### Step 3 – Share the Link

Send the generated URL through your preferred communication platform.

Example:

```text
WhatsApp
Telegram
Signal
Email
```

### Step 4 – Monitor Activity

LinkLook will store generated logs and captured files within the project directory while the session is active.

---

## Cleanup

After testing is complete, remove all generated logs and temporary files:

```bash
bash cleanup.sh
```

This will:

* Remove generated logs
* Delete temporary files
* Clear session data
* Reset the working directory

---

## Directory Structure

```text
LinkLook/
│
├── linklook.sh
├── cleanup.sh
├── sites/
├── logs/
├── captured/
└── README.md
```

---

## Example Workflow

```bash
git clone https://github.com/<your-username>/LinkLook.git

cd LinkLook

chmod +x linklook.sh cleanup.sh

bash linklook.sh

# Copy generated link

# Send via WhatsApp

# After testing
bash cleanup.sh
```

---

## Disclaimer

LinkLook is intended solely for:

* Authorized security awareness demonstrations
* User experience research
* Educational purposes
* Controlled testing environments

Users are responsible for complying with all applicable laws, regulations, and organizational policies. Always obtain proper authorization before conducting any testing activities.

---

## Author

Breached - Mainak

Version: 1.0

Release Notes:

* Initial release
* Added hyper-realistic Zoom Meeting Waiting Room page
* Added Cloudflare Tunnel integration
* Added automated cleanup utility
