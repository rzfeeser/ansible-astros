# ansible-astros


## Overview

This repository contains Ansible playbooks for space data automation:
- `playbook.yml` fetches the current list of astronauts in space.
- `playbook-iss.yml` retrieves the real-time location of the International Space Station (ISS).
Both use the public Open Notify API and save results as local JSON files for further analysis or sharing.


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

2. **Run a playbook:**
	- To fetch astronauts:
	  ```bash
	  ansible-playbook playbook.yml
	  ```
	  Output: `astros.json`
	- To fetch ISS location:
	  ```bash
	  ansible-playbook playbook-iss.yml
	  ```
	  Output: `iss-location.json`

3. **View results:**
	- The output JSON files will be saved in the repository directory.

## Playbook Details

- **playbook.yml**: Fetches astronaut data from the Open Notify API and saves it as `astros.json`.


## GitHub Actions

You can manually trigger the workflow from the GitHub Actions tab using the "Playbook Selector" workflow. When started, you will be prompted to choose which playbook(s) to run:
- Select to run `playbook.yml` (astronauts), `playbook-iss.yml` (ISS location), or both.
- After execution, the resulting JSON files are saved as downloadable workflow artifacts.


## License

This project is open source and available under the GNU General Public License v3.0 (GPLv3).
See [LICENSE](https://www.gnu.org/licenses/gpl-3.0.html) for details.

## Contact & Training

- Author: **rzfeeser**
- Webpages: [rzfeeser.com](https://rzfeeser.com), [iris7.com](https://iris7.com)

For inquiries, collaborations, or professional training on any topics covered in my repositories (including Ansible, automation, cloud, and more), please contact me via my websites above. I offer training and consulting services for all technologies featured in my GitHub projects.
