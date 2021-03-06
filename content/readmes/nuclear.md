---
title: nuclear
date: 2021-04-12T08:09:14+0000
draft: false
---
# Nuclear - poc

An ArkScript Package Manager

## Instructions to Run

* Pre-Requisites
    - Python3.6 or above

* Directions to install
    - Clone the repo
    ```bash
    git clone https://github.com/ArkScript-lang/nuclear
    ```
    - Navigate into the repo
    ```bash
    cd nuclear
    ```
    - Activate a virtual env
    ```shell
    python3 -m venv ./venv
    # windows
    .\venv\Scripts\activate.bat
    # linux
    source ./venv/bin/activate
    ```
    - Install the requirements 
    ```bash
    pip3 install -r requirements.txt
    ```

## Troubleshooting

* If you're facing an issue where you cannot download any more tarballs, you might have been rate limited by GitHub
* To increase the rate limit, generate a [personal access token](https://github.com/settings/tokens)
* add token to nuclear
```bash
nuclear --login --token <YOUR TOKEN HERE>
```

## Commands

* To see the help command

    ```bash
    nuclear -h
    ```

    ```bash
    nuclear --help
    ```
* Authentication ([using Github Access Token](https://github.com/settings/tokens))
    ```bash
     --token TOKEN     GitHub token, required if rate limiting is an issue
    ```

* To Install an ArkScript Package from Github
    ```bash
    nuclear install [-h] [-v VERSION] package
    ```
    - Positional Arguments
    format of the package: 
    ```bash
    user/repo
    ```
    - Optional Arguments
        - show this help message and exit
        ```bash
        -h, --help            
        ```
        - Specify a version for the package
        ```bash
        -v VERSION, --version VERSION
        ```

* To Remove an ArkScript Package
    ```bash
    nuclear remove [-h] [-v VERSION] [-g GLOBALLY] package
    ```
    - Positional Arguments:
    format of the package: 
    ```bash
    user/repo
    ```
    - Optional Arguments

        - show this help message and exit
        ```bash
        -h, --help            
        ```
        - Specify a version for the package
        ```bash
        -v VERSION, --version VERSION
        ```
        - Remove a package from the local repositories. If not specified, remove a package from the current project packages list
        ```bash
        -g GLOBALLY, --globally GLOBALLY
        ```




## Launching tests

```shell
python3 -m tests
```