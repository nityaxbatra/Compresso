# 📦 Compresso - Huffman File Compression Tool

Compresso is a lightweight, web-based file compression and decompression application that leverages **Huffman Encoding** to achieve efficient lossless compression. Upload your text files, compress them with optimal encoding, and decompress them back to their original state—all directly in your browser.

---

## 🌐 Live Demo

**[🚀 Try Compresso Now](https://compresso-eight.vercel.app/)**

Open the live application in your browser to start compressing files immediately!

---

## ✨ Features

- **🎯 Fast Compression**: Uses Huffman Encoding algorithm for efficient compression
- **🔄 Bidirectional**: Compress and decompress files seamlessly
- **📱 Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **🛡️ Lossless Compression**: No data loss—files decompress to their exact original form
- **⚡ Client-Side Processing**: All compression happens in your browser; no backend required
- **📚 Educational**: Includes an info page explaining Huffman Coding concepts
- **🎨 Elegant UI**: Clean, intuitive interface with step-by-step guidance
- **📊 File Format Support**: Currently supports `.txt` files

---

## 🚀 Quick Start

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No installation or backend setup required

### Usage

1. **Open the Application**
   - Open `index.html` in your web browser or deploy to GitHub Pages

2. **Compress a File**
   - Click "Select Your File" and upload a `.txt` file
   - The app analyzes character frequencies and builds a Huffman tree
   - Download your compressed file with the optimal encoding

3. **Decompress a File**
   - Upload a previously compressed file
   - The app detects and reverses the compression
   - Download your original file

4. **Learn More**
   - Visit the "Info" page to understand how Huffman Encoding works

---

## 🏗️ Project Structure

```
Compresso/
├── index.html              # Main compression app interface
├── info.html               # Educational page about Huffman Coding
├── script.js               # Main application logic
├── styles.css              # Application styling
├── codec_implementation.js  # Huffman codec logic
├── heap_implementation.js   # Min-heap data structure
├── README.md               # This file
├── dump.md                 # Project documentation
│
├── assets/                 # Icons and sample files
│   ├── text_file_icon1.png
│   ├── done_icon1.jpg
│   ├── options_icon1.png
│   ├── wait_icon1.png
│   ├── SAMPLE1.TXT         # Sample files for testing
│   ├── sample2.txt
│   ├── sample3.txt
│   └── ...
│
└── screenshots/            # UI screenshots
    ├── indexss.png
    ├── compressionss.png
    ├── decompressionss1.png
    ├── infoss1.png
    └── ...
```

---

## 🛠️ Tech Stack

| Technology            | Purpose                                    |
| --------------------- | ------------------------------------------ |
| **HTML5**             | Markup and structure                       |
| **CSS3**              | Styling and responsive design              |
| **JavaScript (ES6+)** | Compression logic and UI interactions      |
| **Huffman Algorithm** | File compression encoding                  |
| **Min-Heap**          | Binary tree construction for Huffman codes |

---

## 📋 How It Works

### Huffman Encoding Algorithm

1. **Frequency Analysis**: Analyzes character frequencies in the input file
2. **Tree Construction**: Builds a binary tree using a min-heap with characters as leaf nodes
3. **Code Generation**: Generates unique binary codes for each character (shorter codes for frequent characters)
4. **Encoding**: Replaces characters with their binary codes
5. **Compression**: Saves the Huffman tree and encoded data

### Decompression

1. **Tree Reconstruction**: Rebuilds the Huffman tree from the stored data
2. **Decoding**: Traverses the tree to convert binary codes back to original characters

---

## 📁 Key Files Explained

### Core Implementation

- **`codec_implementation.js`**
  - Implements the Huffman codec class
  - Methods: `getCodes()`, `make_string()`, `make_tree()`
  - Handles both compression and decompression logic

- **`heap_implementation.js`**
  - Implements a min-heap data structure
  - Used for building the Huffman tree efficiently
  - Supports heap operations: insert, extract-min, heapify

- **`script.js`**
  - Manages file upload and user interactions
  - Coordinates compression/decompression workflow
  - Handles file download and error handling

### UI Files

- **`index.html`**
  - Main compression interface
  - Three-step workflow: Select → Compress/Decompress → Download

- **`info.html`**
  - Educational resource explaining Huffman Coding
  - Visual explanation of the algorithm

- **`styles.css`**
  - Modern, responsive design
  - Mobile-friendly layout
  - Clean typography using Poppins font

---

## 🎯 Workflow

### Compression Workflow

```
Input File (.txt)
    ↓
File Upload
    ↓
Frequency Analysis
    ↓
Huffman Tree Construction
    ↓
Generate Binary Codes
    ↓
Encode Content
    ↓
Compressed File (.txt)
    ↓
Download
```

### Decompression Workflow

```
Compressed File
    ↓
File Upload
    ↓
Detect Huffman Format
    ↓
Reconstruct Huffman Tree
    ↓
Decode Binary Data
    ↓
Original File (.txt)
    ↓
Download
```

---

## 💾 File Format

Compressed files include:

- **Huffman Tree Structure**: Serialized tree representation
- **Encoded Data**: Binary-encoded file content
- **Metadata**: File information for decompression

---

## 🧪 Testing

Sample text files are provided in the `assets/` folder:

- `SAMPLE1.TXT`
- `sample2.txt` through `sample14.txt`

Use these to test compression ratios and verify the decompression accuracy.

---

## 🚀 Deployment

This is a static web application with no backend requirements.

### Deploy to GitHub Pages

1. Push your repository to GitHub
2. Go to repository Settings → Pages
3. Select the `main` branch as the publishing source
4. Your app will be available at `https://username.github.io/repo-name`

### Deploy to Other Platforms

- **Netlify**: Drag-and-drop the folder
- **Vercel**: Connect your GitHub repository
- **Firebase Hosting**: Use the Firebase CLI
- **Any Static Host**: Upload the files as-is

---

## 🎓 Learning Resources

Visit the **Info** page in the application to learn about:

- How Huffman Encoding works
- Why it's efficient for compression
- Real-world applications
- Complexity analysis

---

## 📊 Performance Characteristics

- **Time Complexity**: O(n log n) for compression where n = number of unique characters
- **Space Complexity**: O(n) for the Huffman tree
- **Compression Ratio**: Varies by file content; text files typically compress 30-50%

---

## 🔐 Security & Privacy

- ✅ All processing happens client-side in your browser
- ✅ No data is sent to any server
- ✅ Files never leave your device
- ✅ Completely secure and private

---

## 🐛 Known Limitations

- Currently supports `.txt` files only
- Very small files may expand slightly due to tree overhead
- Large files (>50MB) may impact browser performance

---

## 🤝 Contributing

Contributions are welcome! Potential improvements:

- Support for more file types (PDF, images, archives)
- Compression ratio statistics
- Batch file compression
- Different encoding algorithms (LZ77, DEFLATE)
- Advanced statistics and visualization

---

## 👨‍💻 Author

**Nitya Batra**  
[GitHub Profile](https://github.com/nityaxbatra)

---

## 📄 License

This project is open source and available for educational and commercial use.

---

## 🙋 Support & Questions

- Check the **Info** page for algorithm explanations
- Review the code comments in `codec_implementation.js` and `heap_implementation.js`
- Test with provided sample files in the `assets/` folder

---

## 📸 Screenshots

The `screenshots/` folder contains visual documentation of:

- Main interface
- Compression process
- Decompression results
- Responsive design on different devices
- Information pages

---

**Happy Compressing! 🎉**
