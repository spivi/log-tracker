# Log Insights PyCharm Plugin

## Overview

Log Insights is a PyCharm plugin designed to help developers manage and document log messages in their Python projects. It provides an easy way to view, edit, and export log messages, focusing on changes made in the current Git branch compared to the master branch.

## Features

- **Log Message Tracking**: Automatically detects log messages in Python files modified in the current Git branch.
- **In-IDE Documentation**: Allows adding and editing descriptions for log messages directly within PyCharm.
- **Export Functionality**: Exports log messages and their descriptions to a Markdown file for easy sharing and documentation.
- **Git Integration**: Focuses on log messages in files that have been modified in the current branch compared to the master branch.
- **Real-time Updates**: Refreshes log messages when switching Git branches or on-demand.

## Installation

1. Open PyCharm IDE
2. Go to `File` > `Settings` > `Plugins` (on macOS, `PyCharm` > `Preferences` > `Plugins`)
3. Click on "Marketplace" and search for "Log Insights"
4. Click "Install" and restart PyCharm when prompted

## Usage

1. After installation, you'll find a new tool window labeled "Log Insights" on the right side of your PyCharm IDE.
2. The tool window displays a tree view of log messages found in your modified Python files.
3. Double-click on a log message to add or edit its description.
4. Use the "Refresh" button to update the list of log messages.
5. Use the "Export to Markdown" button to generate a Markdown file containing all log messages and their descriptions.

## Development

### Prerequisites

- IntelliJ IDEA
- Java Development Kit (JDK) 11 or later
- Gradle

### Setup

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/log-insights-plugin.git
   ```
2. Open the project in IntelliJ IDEA
3. Import the project as a Gradle project
4. Run the `buildPlugin` Gradle task to build the plugin
5. Run the `runIde` Gradle task to test the plugin in a sandbox environment

### Project Structure

- `src/main/java/com/example/loginsights/`: Contains the main Java source files
- `src/main/resources/`: Contains resource files, including `META-INF/plugin.xml`
- `src/test/java/com/example/loginsights/`: Contains test files

### Key Components

- `LogInsightsToolWindow`: Manages the tool window integration with PyCharm
- `LogInsightsPanel`: Implements the main UI of the plugin
- `GitLogAnalyzer`: Handles Git integration to find modified files
- `LogParser`: Parses Python files to extract log messages
- `LogMessage`: Represents a single log message with its metadata

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Support

If you encounter any issues or have questions, please file an issue on the GitHub issue tracker.