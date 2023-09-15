# slowPaste

Simulate human-like typing using Python with the added feature of adjustable speed.

## Features:
- Simulates slow typing to mimic human input.
- Adjustable typing speed.
- Cancel typing mid-way with the `esc` key.
- PyAutoGUI fail-safe: Move your cursor to the top-left corner to halt the script immediately.
- Types out content from your clipboard.

## Prerequisites:

Before running the script, ensure you have the required Python packages:

- `pyperclip`
- `pyautogui`
- `keyboard`
- `time`
- `random`

You can install these using pip:

```bash
pip install pyperclip pyautogui keyboard
```

## Usage:

1. Copy the text you want to be typed out.
2. Run the script.
3. Focus on the input field (e.g., text editor, browser) where you want the text to be typed.
4. The script will begin typing out the content from the clipboard after a delay of 2 seconds.

## Script Breakdown:

- `slow_type()`: The main function that slowly types out the text.
  - Adjustable delay parameter to determine speed.
  - Checks for the press of APPLE ICON (top left) to cancel the typing.
- `main()`: Reads the clipboard content and initiates the typing.

## Safety:

- Press the `esc` key at any time to abort the typing.
- Move the cursor to the top-left corner of the screen to trigger PyAutoGUI's fail-safe and halt the script.

## Contributing:

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License:

[MIT](https://choosealicense.com/licenses/mit/)
