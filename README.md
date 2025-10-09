# TheOne LocalData Editor

**Editor tools for managing local user data in Unity**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Unity](https://img.shields.io/badge/Unity-2021.3%2B-blue.svg)](https://unity3d.com/get-unity/download)
[![UPM](https://img.shields.io/badge/UPM-Registry-green.svg)](https://upm.the1studio.org)

## Overview

This package provides comprehensive tools for viewing, editing, and debugging local data storage used by UITemplate, including PlayerPrefs and custom data systems. Essential for debugging and testing user data persistence.

## Features

- **Data Viewer**: Browse all stored local data in a clean interface
- **Data Editor**: Modify PlayerPrefs and custom data values directly in the editor
- **Bulk Operations**: Clear all data or specific categories with one click
- **Import/Export**: Backup and restore local data for testing
- **Real-time Monitoring**: Watch data changes during play mode
- **Type Support**: Handle strings, integers, floats, and boolean values
- **Search & Filter**: Quickly find specific data keys

## Requirements

- Unity 2021.3 or higher
- Addressables Package 1.19.0+
- Cysharp.UniTask 2.3.0+
- Unity Localization 1.3.0+
- TextMeshPro 3.0.0+
- TheOne Extensions 1.0.0+
- TheOne Tool Core 1.0.0+

## Installation

### Via UPM Registry (Recommended)

Add to your `Packages/manifest.json`:

```json
{
  "dependencies": {
    "com.theone.tool.localdata": "1.0.0"
  },
  "scopedRegistries": [
    {
      "name": "TheOne Studio",
      "url": "https://upm.the1studio.org",
      "scopes": ["com.theone"]
    }
  ]
}
```

### Via Git URL

```json
{
  "dependencies": {
    "com.theone.tool.localdata": "https://github.com/The1Studio/UITemplateLocalData.git"
  }
}
```

## Usage

### Accessing the Tool

**Menu**: `TheOne → Configuration And Tools → LocalData Tab`

### Common Operations

#### View All PlayerPrefs

Open the LocalData tab to see all stored PlayerPrefs with their keys and values.

#### Edit a Value

1. Locate the key in the list
2. Click on the value field
3. Enter new value
4. Changes are applied immediately

#### Clear All Data

Use the "Clear All" button to delete all PlayerPrefs (useful for testing fresh installs).

#### Export Data

Export current PlayerPrefs to a JSON file for backup or testing purposes.

#### Import Data

Import previously exported data to restore a specific state.

## API Reference

### LocalDataEditor

Main editor window for managing local data. Access via Unity menu or:

```csharp
using TheOne.Tool.LocalData;

// Programmatic access
LocalDataEditor.ShowWindow();
```

## Best Practices

1. **Backup Before Clearing**: Always export data before clearing in production builds
2. **Testing Fresh Install**: Use "Clear All" to test first-time user experience
3. **Debug Builds Only**: Avoid shipping debug data tools in production builds
4. **Data Migration**: Use export/import for testing data migration scenarios

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## About The One Studio

**The One Studio** is a mobile game development company specializing in hypercasual and casual games.

- Website: [https://the1studio.com](https://the1studio.com)
- Email: contact@the1studio.com

## Related Packages

- [UITemplate](https://github.com/The1Studio/UITemplate) - Complete Unity UI framework
- [TheOne Template Editor](https://github.com/The1Studio/UITemplateEditorCore) - Core editor tools
- [Unity Optimization Tools](https://github.com/The1Studio/UnityOptimizationTools) - Project optimization
- [TheOne Localization](https://github.com/The1Studio/UITemplateLocalization) - Localization tools

## Support

- [GitHub Issues](https://github.com/The1Studio/UITemplateLocalData/issues)
- [Documentation](https://github.com/The1Studio/UITemplateLocalData#readme)

---

<div align="center">

Made with ❤️ by **The One Studio**

</div>
