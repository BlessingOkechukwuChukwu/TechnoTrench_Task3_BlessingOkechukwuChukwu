# Basic Vulnerability Scanner

This Python script implements a basic vulnerability scanner that checks for open ports on a given IP address and identifies potential security vulnerabilities based on the services running on those ports.

## Features

- Scans a range of ports on a specified IP address
- Identifies open ports and attempts to determine the services running on them
- Checks for common vulnerabilities associated with certain open ports
- Provides a report of open ports and potential vulnerabilities

## Requirements

- Python 3.x

## Installation

1. Ensure you have Python 3.x installed on your system.
2. Download the `vulnerability_scanner.py` script to your local machine.

## Usage

Run the script from the command line, providing the IP address you want to scan as an argument:

```
python3 vulnerability_scanner.py <ip_address>
```

Replace `<ip_address>` with the IP address you want to scan.

Example:
```
python3 vulnerability_scanner.py 192.168.1.1
```

## Output

The script will display:
- A list of open ports and the services running on them
- Potential vulnerabilities associated with the open ports

## Important Notes

- This is a basic scanner and may not detect all vulnerabilities.
- Only use this scanner on networks and systems you own or have explicit permission to test.
- Scanning networks without permission may be illegal in some jurisdictions.
- The script currently scans ports 1-1024 by default. You can modify the `end_port` variable in the script to scan more ports, but this will increase scan time.

## Limitations

- The vulnerability checks are basic and based on commonly known issues associated with certain ports.
- The script does not perform deep inspection of services or attempt to exploit vulnerabilities.
- Service identification is based on standard port assignments and may not always be accurate.

## Legal Disclaimer

This tool is provided for educational and ethical testing purposes only. The user assumes all responsibility for the use of this tool. The authors are not responsible for any misuse or damage caused by this program.

## Contributing

This is a basic implementation. Feel free to fork the project and enhance its capabilities. Some potential improvements could include:
- Adding more comprehensive vulnerability checks
- Implementing version detection for identified services
- Adding options for output formats (e.g., JSON, CSV)
- Improving scanning speed and efficiency
