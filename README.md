# Water Reminder Notification Script

A minimal Python script that sends you hourly desktop notifications reminding you to drink water. It loops forever, prints a console reminder, and uses the `plyer` library to trigger system notifications. 

---

## Features

* Sends a desktop notification every hour.
* Prints a reminder message in the console.
* Uses `plyer.notification.notify` for cross-platform alerts.
* Runs indefinitely until manually stopped.

---

## How It Works

1. Imports `time` and `notification` from `plyer`.
2. Runs a `while True` loop that continuously:

   * Prints: `"Please sip some water!"`
   * Sends a notification:

     ```python
     notification.notify(
         title="Please drink some water",
         message="You need to drink some water"
     )
     ```


   * Sleeps for one hour: `time.sleep(60*60)`

---

## Installation

### Install dependencies:

```bash
pip install plyer
```

---

## Usage

Run the script:

```bash
python main.py
```

You will receive a desktop notification every hour.

---

## Requirements

* Python 3.x
* `plyer` library
* Desktop environment that supports system notifications

---

