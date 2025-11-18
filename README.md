
# YOLO Label Editor

A highly flexible interactive web-based tool for visualizing, editing, and managing YOLO format bounding box labels. Download and run the html file on your local system for 100% Privacy. No data leaves your server.

## 🚀 [Launch Application](https://EliMahMD.github.io/yolo-label-editor/)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![No Dependencies](https://img.shields.io/badge/dependencies-none-green.svg)](https://github.com/yourusername/yolo-label-editor)

## ✨ Features

### 🖼️ Image Support
- **Multiple Format Support**: `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.webp`, `.nii.gz`
- **Batch Processing**: Upload and edit multiple image-label pairs simultaneously
- **Navigation**: Easy switching between image pairs with Previous/Next buttons
- **High Resolution**: Supports images of any size with automatic canvas scaling

### 🏷️ Label Management
- **YOLO Format**: Standard YOLO format (`class_id center_x center_y width height`)
- **Real-time Interactive Editing**: Edit either of coordinate values in text editor or bounding box corners on the image
- **Custom Class Names**: Map class IDs to human-readable names
- **Visibility Toggles**: Show/hide individual labels or all labels at once

### 📁 File Operations
- **Automatic Pairing**: Matches images and labels by filename (e.g., `image.jpg` ↔ `image.txt`)
- **Batch Upload**: Select multiple files at once
- **Custom Output Path**: Specify a path + prefix for downloaded files or leave it empty for mainting the original name
- **Save Current**: Export currently edited labels
- **Save All**: Export all labels from all image pairs at once

### 🔒 Privacy & Security
- **100% Local Processing**: All operations run in your browser
- **No Server Required**: No data transmission to any server
- **Offline Capable**: Works completely offline after initial page load
- **No Installation**: Pure HTML/JavaScript - no dependencies to install

## 📖 User Guide

### Getting Started

1. **Open the Application**
   - Click the launch link above or open `index.html` in your browser
   - No installation or setup required

2. **Upload Files**
   - Click "Upload Multiple Image-Label Pairs"
   - Select both image files and their corresponding `.txt` label files
   - Files are automatically matched by basename (e.g., `scan001.nii.gz` + `scan001.txt`)

3. **Start Editing**
   - Labels are initially hidden - toggle visibility as needed
   - Click boxes to select them
   - Drag to move or resize

**Use Cases:**
- Focus on specific objects by hiding others
- Reduce visual clutter
- Check individual label accuracy


## 🎨 Interface Overview

```
┌─────────────────────────────────────────────────────┐
│            YOLO Label Editor                        │
│        Upload image-label pairs to begin            │
├─────────────────────────────────────────────────────┤
│  [Upload Multiple Image-Label Pairs]                │
├─────────────────────────────────────────────────────┤
│  [Previous] 1/10 - image001 [Next]  Output: [path] │
│  [Save Current] [Save All]                          │
├─────────────────────────────────────────────────────┤
│  Class Names (Optional)                             │
│  ┌─────────────────────────────────────┐            │
│  │ person                              │            │
│  │ car                                 │            │
│  │ ...                                 │            │
│  └─────────────────────────────────────┘            │
├──────────────────────┬──────────────────────────────┤
│   Image Preview      │    YOLO Labels               │
│  ┌─────────────────┐ │  ┌─────────────────────────┐ │
│  │                 │ │  │ 0 0.5 0.5 0.3 0.4       │ │
│  │   [Image with]  │ │  │ 1 0.3 0.3 0.2 0.2       │ │
│  │   [Bounding]    │ │  │ ...                     │ │
│  │   [Boxes]       │ │  └─────────────────────────┘ │
│  │                 │ │                              │
│  └─────────────────┘ │  Label Visibility Controls:  │
│  0/3 visible         │  ☐ Box 1 (person) [👁️]      │
│  [Show All][Hide All]│  ☐ Box 2 (car) [👁️]         │
│                      │  ☐ Box 3 (dog) [👁️]         │
└──────────────────────┴──────────────────────────────┘
```

### Browser Compatibility

- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera
- ⚠️  IE 11 (not supported)

## 🐛 Troubleshooting

### Labels not showing?
- Check that labels start hidden - click "Show All" button
- Verify YOLO format is correct (5 values per line)
- Ensure coordinates are between 0 and 1

### Files not matching?
- Ensure image and label files have identical basenames
- Example: `image.jpg` matches `image.txt`, not `image_labels.txt`
- File extensions: `.nii.gz` → remove `.nii.gz`, `.jpg` → remove `.jpg`

### Can't drag boxes?
- Make sure box is visible (eye icon on)
- Click to select box first (turns red)
- Drag from inside box to move, from handles to resize

### Download not working?
- Check browser allows downloads
- Try different browser if issues persist
- File saves to default downloads folder

## 🤝 Contributing

Contributions are welcome! 

## 📜 License

MIT License - feel free to use this tool for any purpose.

## 🙏 Acknowledgments

- Built with React and Tailwind CSS
- Inspired by the need for simple, privacy-focused labeling tools
- Thanks to the YOLO community

## 📞 Support

For issues, questions, or suggestions:
- Open an issue on GitHub
- Check existing issues for solutions
- Contribute improvements via pull requests

## 🔮 Roadmap

Potential future features:
- [ ] Undo/redo functionality
- [ ] Box creation (draw new boxes)
- [ ] Box deletion
- [ ] Zoom and pan for large images
- [ ] Export to other formats (COCO, Pascal VOC)
- [ ] Batch operations (delete all Class X)

---

**Made with ❤️ for the computer vision community**

**[⭐ Star this repo](https://github.com/YOUR-USERNAME/yolo-label-editor)** if you find it useful!
