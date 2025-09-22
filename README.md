# ansible-astros

## Overview

This repository provides an Ansible playbook to fetch the current list of astronauts in space using the [Open Notify API](http://api.open-notify.org/astros.json). The playbook retrieves the data and saves it locally as a JSON file.


## Author

Repository maintained by [rzfeeser](#contact--training).

## Prerequisites

- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) installed on your system
- Internet access to reach the Open Notify API

## Usage

1. **Clone the repository:**
	```bash
	git clone https://github.com/rzfeeser/ansible-astros.git
	cd ansible-astros
	```

2. **Run the playbook:**
	```bash
	ansible-playbook playbook.yml
	```

3. **Result:**
	- The playbook will fetch the current astronauts and save the result to `astros.json` in the repository directory.

## Playbook Details

- **playbook.yml**: Fetches astronaut data from the Open Notify API and saves it as `astros.json`.

## GitHub Actions

- Commits with the word `astros` run `playbook.yml`.
- Commits with the word `iss` run `playbook-iss.yml` (to be created).


## License

This project is open source and available under the GNU General Public License v3.0 (GPLv3).
See [LICENSE](https://www.gnu.org/licenses/gpl-3.0.html) for details.

## Contact & Training

- Author: **rzfeeser**
- Webpages: [rzfeeser.com](https://rzfeeser.com), [iris7.com](https://iris7.com)

For inquiries, collaborations, or professional training on any topics covered in my repositories (including Ansible, automation, cloud, and more), please contact me via my websites above. I offer training and consulting services for all technologies featured in my GitHub projects.
