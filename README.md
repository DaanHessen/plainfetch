# plainfetch

*Your system info, plain and simple.*

### About

`plainfetch` is a lightweight, no-frills system information tool for minimalists. It's written in simple shell script, making it blazingly fast and easy to understand and modify.

Unlike other fetch tools, `plainfetch` doesn't bother with ASCII art or overly complex details. It does one thing and does it well: it shows you the essential information about your system in a clean, uncluttered way. It is designed to be POSIX-compliant, so it should run on virtually any system with a standard shell.

### Features

* **Minimalist Design:** Just the information you need, nothing you don't.
* **Blazingly Fast:** Runs instantly with no noticeable delay.
* **Highly Customizable:** Easily change labels and colors through a simple configuration file.
* **Lightweight:** No dependencies outside of standard system utilities.
* **POSIX-compliant:** Built to run anywhere without requiring `bash` or `zsh`.

### Installation

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/your-username/plainfetch.git](https://github.com/your-username/plainfetch.git)
    cd plainfetch
    ```

2.  **Make the script executable:**
    ```sh
    chmod +x plainfetch
    ```

3.  **Place it in your PATH:**
    Move the executable to a directory in your system's PATH to make it available everywhere. `/usr/local/bin` is a great choice.
    ```sh
    sudo mv plainfetch /usr/local/bin/
    ```

### Configuration

`plainfetch` is configured with a simple text file.

1.  **Create the config directory and copy the file:**
    ```sh
    mkdir -p ~/.config/plainfetch
    cp config ~/.config/plainfetch/
    ```

2.  **Edit the config file:**
    Open `~/.config/plainfetch/config` with your favorite text editor. The format is simple key-value pairs.

    **Example `config` file:**
    ```sh
    # This is a comment.
    # Change the label text for each info line.
    # Leave a value empty to hide the line.
    #
    # Supported colors: black, red, green, yellow, blue, magenta, cyan, white

    # Labels
    LABEL_OS="System"
    LABEL_KERNEL="Kernel"
    LABEL_UPTIME="Uptime"
    LABEL_MEM="RAM"
    LABEL_CPU="Processor"
    LABEL_DISK="Storage"

    # Colors
    COLOR_LABEL="blue"
    COLOR_TEXT="white"
    ```

### Usage

Simply run the command in your terminal:
```sh
plainfetch
```

### Contributing

Contributions are welcome! If you have an idea for an improvement or find a bug, feel free to open an issue or submit a pull request.

### License

Licensed under the MIT License.
