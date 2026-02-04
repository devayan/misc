# CLAUDE.md

This file provides guidance for Claude Code when working with this repository.

## Repository Overview

This is a collection of miscellaneous scripts, utilities, and code snippets primarily written in Python and C. The code covers various domains including security research, web scraping, network utilities, and Windows system tools.

## Project Structure

```
misc/
├── *.py                          # Standalone Python scripts
├── *.c                           # Standalone C programs (Windows-focused)
├── mail_return_receipt/          # PHP-based email tracking tool
├── mod_evil_shell_backdoor/      # Apache module reverse shell (C/VB)
├── network_clipboard_sync/       # .NET clipboard synchronization tool
└── vmware_controller_gui/        # VMware control GUI application
```

## Code Categories

### Security/Exploit Research (Python)
- `*_exploit.py` - Proof-of-concept exploits for security research
- Educational/CTF context only

### Web Scrapers (Python)
- `*_scraper.py`, `*_download.py` - Content extraction scripts
- Uses libraries: requests, BeautifulSoup, urllib

### Network Utilities (Python)
- `nmap_normaloutput_parse.py` - Nmap output parser
- `tor_exit_nodes_list.py` - Tor exit node enumeration
- `ymsg_parser_scapy.py` - Yahoo messenger protocol parser

### Windows Tools (C)
- `pe_summary_view.c` - PE file analyzer
- `read_process_memory.c` - Process memory reader
- `windows_*.c` - Various Windows system utilities

## Development Notes

- Python scripts are standalone and use Python 2/3 compatible syntax
- C programs target Windows API (compile with MSVC or MinGW)
- No package manager or build system - scripts are independent
- No test suite exists

## Common Commands

```bash
# Run a Python script
python <script_name>.py

# Compile C programs (Windows/MinGW)
gcc -o output.exe source.c -lws2_32  # for network code
gcc -o output.exe source.c           # for basic utilities
```
