# mHome - Home Assistant Add-on

<p align="center">
  <img src="logo.png" alt="mHome Logo" width="200">
</p>

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]

A Home Assistant add-on that serves as mHome local Hub, providing seamless integration between your Home Assistant instance and the mHome cloud service.

## About

This add-on bridges your local Home Assistant installation with the mHome cloud service, enabling:

- **Continuous Operation**: Runs as a background service maintaining persistent connections
- **Cloud Integration**: Keeps a websocket connection to the mHome cloud for real-time data synchronization
- **Local-to-Cloud Bridge**: Seamlessly transfers local device data to mHome cloud services
- **Future Local Engine**: Upcoming feature to process automations entirely locally
- **External Data Integration**: Bridge external data sources to your local automation engine

## Installation

### Method 1: One-Click Installation

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fmhome-ai%2Fha-addon)

### Method 2: Manual Installation

1. Navigate to **Settings** > **Add-ons** > **Add-on Store** in Home Assistant
2. Click the **⋮** menu in the top right corner and select **Repositories**
3. Add this repository URL: `https://github.com/mhome-ai/ha-addon`
4. Click **Add** and wait for the repository to be processed
5. Find "mHome" in the add-on store and click **Install**

### Method 2: Manual Installation

1. Download the latest release from this repository
2. Extract to your Home Assistant's `addons` directory
3. Restart Home Assistant
4. Navigate to **Settings** > **Add-ons** > **Add-on Store**
5. Find "mHome" in the **Local add-ons** section and click **Install**

## Configuration

The add-on requires minimal configuration. After installation:

1. Start the add-on
2. Check the **Log** tab for any configuration requirements
3. The add-on will automatically connect to the mHome cloud service

### Configuration Options

```yaml
# No configuration options currently available
# Configuration will be added in future versions
```

## Usage

Once installed and started, the add-on will:

1. Establish a connection to the mHome cloud service
2. Begin monitoring your Home Assistant entities
3. Sync data between your local instance and the cloud
4. Provide a local web interface on port 8080 (if configured)

## Support

For issues and feature requests, please:

1. Check the add-on logs for error messages
2. Open an issue on [GitHub](https://github.com/mhome-ai/ha-addon/issues)

## License

This project is licensed under the MIT License.

## Changelog

### Version 0.1.0
- Initial release
- Basic cloud connectivity
- Home Assistant integration
- Multi-architecture support

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg 