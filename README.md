# Satellite Quickstart

This repository is designed to be an introduction to Red Hat Satellite, the redhat.satellite ansible collection, and treating Satellite as code. The intention is to have a presentation explaining the component of satellite being configured or modified, and the code to do that action. Included is a playbook and some pre-defined options and variables.

## Usage

First install the requirements with ansible galaxy: `ansible-galaxy collection install collections/requirements.yml`

Then create a quick inventory file and select an option from the table below:
```yaml
---
[satellite]
satellite01.domain.lcl quickstart_option=reference
satellite02.domain.lcl quickstart_option=101
```

### Quickstart Options ###
The variable that controls what runs is defined as `quickstart_option`. See below for valid definitions and descriptions:
| Name        | Description               | Target Audience                                                                     |
|-------------------------------------------------------------------------------------------------------------------------------|
| `101`       | Introduction to Satellite | Anyone interested in Satellite, no experience required. Paired with a presentation  |
| `reference` | Reference Satellite Setup | Anyone interested in seeing a Satellite that conforms to "best practices"           |
