<div align="center">
    <h1>
        ConfiScan
    </h1>
    <p align="center">
        Collect basic information about Linux systems within seconds.
        <br/>
        <strong>·</strong>
        <a href="https://github.com/AntonVanAssche/ConfiScan/issues">Report Bug</a>
        <strong>·</strong>
        <a href="https://github.com/AntonVanAssche/ConfiScan/issues">Request Feature</a>
    </p>
    <p align="center">
        <a href="https://github.com/AntonVanAssche/ConfiScan/graphs/contributors">
            <img src="https://img.shields.io/github/contributors/AntonVanAssche/ConfiScan.svg?style=for-the-badge">
        </a>
        <a href="https://github.com/AntonVanAssche/ConfiScan/releases/latest/">
            <img src="https://img.shields.io/github/release/AntonVanAssche/ConfiScan.svg?style=for-the-badge">
        </a>
        <a href="https://github.com/AntonVanAssche/ConfiScan/network/members">
            <img src="https://img.shields.io/github/forks/AntonVanAssche/ConfiScan.svg?style=for-the-badge">
        </a>
        <a href="https://github.com/AntonVanAssche/ConfiScan/stargazers">
            <img src="https://img.shields.io/github/stars/AntonVanAssche/ConfiScan.svg?style=for-the-badge">
        </a>
        <a href="https://github.com/AntonVanAssche/ConfiScan/issues">
            <img src="https://img.shields.io/github/issues/AntonVanAssche/ConfiScan.svg?style=for-the-badge">
        </a>
        <a href="https://github.com/AntonVanAssche/ConfiScan/blob/master/LICENSE">
            <img src="https://img.shields.io/github/license/AntonVanAssche/ConfiScan.svg?style=for-the-badge">
        </a>
</div>

## About ConfiScan

> :warning: Currently, only Debian is supported. Support for other Linux distributions will be added soon.

**ConfiScan** is a Bash script designed to collect basic information about Linux systems and output it into a set of organized files. This tool is intended to assist system administrators in documenting and managing their infrastructure, providing a clear and comprehensive overview of system configurations.

The tool was initially developed as part of a bachelor thesis aimed at exploring solutions to facilitate the transition to Infrastructur as Code environments. Recognizing the ongoing challenges that many small and medium-sized enterprises (SMEs) face, such as limited knowledge, time, and budget constraints, ConfiScan will continue to be developed within this repository. It provides a straightforward and effective method for collecting and organizing system information, simplifying the creation of a comprehensive configuration inventory.

More information about the initial script and backstory can be found at the [repository containing the thesis](https://github.com/AntonVanAssche/hogent-bachelorproef/).

## Usage

### Prerequisites

To use ConfiScan, you need the following:

- Packages:
    - `dmidecode`
    - `net-tools`
- Sudo privileges to execute system commands.

### Execution

```console
$ confiscan.sh -h
Usage: confiscan.sh [OPTION] [CONFIG_FILES]

Options:
    -h   Display help
    -t   Create tarball of output directory

Note:
    Shell globbing is supported for [CONFIG_FILES]. They can be files or directories.

Examples:
    confiscan.sh -h
    confiscan.sh /etc/sysctl.conf
    confiscan.sh /etc/apache2/ /etc/sysctl.conf
    confiscan.sh -t /etc/bash{.bashrc,_completion}
    confiscan.sh -t
```

## Contributions

Contributions are welcome! Refer to [`CONTRIBUTING.md`](./CONTRIBUTING.md) for more information on how to contribute.

## License

ConfiScan is licensed under the GPLv3 License. See the [`LICENSE`](./LICENSE) file for more details.
