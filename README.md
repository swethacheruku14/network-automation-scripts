# Network Automation Toolkit

A Python-based Network Automation Toolkit designed to simplify and automate common network engineering tasks across Cisco network devices.

This repository contains automation scripts for network configuration, device monitoring, troubleshooting, compliance validation, configuration management, and operational health checks.

The goal is to reduce repetitive manual CLI operations, improve operational efficiency, and provide consistent network management through Python automation.

## Project Modules

The repository is organized into the following automation modules:

| Module | Description |
|---|---|
| `BGP_Neighbor_Monitoring` | Automates monitoring and verification of BGP neighbor status and connectivity. |
| `BGP_Lab_Rebuild` | Contains scripts for rebuilding and configuring BGP lab environments. |
| `Pre_Post_Change_Validation` | Performs network validation before and after configuration changes. |
| `Multi_Device_Deployment` | Automates configuration deployment across multiple network devices. |
| `Interface_Configuration` | Automates interface configuration and IP address assignments. |
| `Health_Check` | Collects device health information, including CPU, memory, interfaces, BGP, and OSPF status. |
| `Config_Backup` | Automates network device configuration backup operations. |
| `Compliance_Check` | Validates network device configurations against predefined compliance requirements. |
| `VLAN_Configuration` | Automates VLAN creation and configuration on network devices. |
| `Routing_Protocols_Health_Check` | Performs health checks for routing protocols and verifies neighbor relationships. |
| `BGP_Configuration` | Automates BGP configuration and neighbor establishment. |

## Technologies Used

- **Python 3** – Core automation language.
- **Netmiko** – SSH-based network device connectivity and CLI automation.
- **PyYAML** – YAML-based device inventory and configuration management.
- **ThreadPoolExecutor** – Concurrent execution of automation tasks across multiple devices.
- **Cisco IOS** – Network device operating system used for automation examples.

## Prerequisites

Before running the automation scripts, ensure the following are installed:

- Python 3.9+
- pip
- SSH connectivity to the target network devices.
- Appropriate device credentials and privilege permissions.

### Install Dependencies

```bash
pip install netmiko pyyaml
```

Install any additional dependencies required by individual modules.

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/swethacheruku14/network-automation-scripts.git
```

### 2. Navigate to the Project

```bash
cd network-automation-scripts
```

### 3. Configure Device Inventory

Update the YAML inventory files with the required network device information.

Example:

```yaml
routers:
  - device_type: cisco_ios
    host: 192.168.1.1
    username: admin
    password: your_password
```

Use the inventory format expected by each individual script.

### 4. Execute Automation Scripts

Navigate to the required module directory and execute the corresponding Python script.

```bash
cd Health_Check
python health_check.py
```

Replace the script name with the actual entry-point filename in the respective module.

## Key Automation Capabilities

- Automated network device configuration.
- BGP neighbor configuration and monitoring.
- VLAN and interface provisioning.
- Multi-device configuration deployment.
- Network device health monitoring.
- Configuration backup and validation.
- Pre-change and post-change verification.
- Routing protocol health checks.
- Configuration compliance validation.
- Concurrent execution across multiple network devices.

## Security Considerations

- Do not hardcode production credentials in Python scripts.
- Avoid committing passwords, SSH keys, or sensitive device information.
- Use environment variables or secure credential management.
- Restrict automation access to authorized network devices.
- Test configuration changes in a lab environment before deploying to production.

## Future Enhancements

- Add structured logging and centralized execution reports.
- Integrate automated configuration rollback.
- Extend support for additional network vendors.
- Implement REST API-based network automation.
- Integrate Ansible for configuration management.
- Add automated network topology discovery.
- Develop a centralized dashboard for monitoring automation results.

## Disclaimer

This repository is intended for learning, experimentation, and practical network automation use cases. Always validate scripts in a controlled lab environment before executing them against production infrastructure.

## Author

**Swetha Cheruku**

Network Automation | Python | Cisco Networking | Infrastructure Automation
