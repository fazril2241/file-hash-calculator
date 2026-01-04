STILL ON WORK!!

![Python](https://img.shields.io/badge/Python-3.7%2B-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Tool-red)
![CLI](https://img.shields.io/badge/CLI-Tool-brightgreen)

```markdown
 🔐 File Hash Calculator
> A powerful command-line tool for calculating and verifying file hashes.
Essential for cybersecurity professionals, digital forensics, and file integrity verification.

 ✨ Features

- 🔐 Multiple Algorithms: MD5, SHA1, SHA256, SHA512
- ⚡ Progress Bar: Visual feedback for large files
- ✅ Hash Verification: Compare calculated hash with expected value
- 💾 Result Saving: Save hash results to text files
- 🖥️ Command Line Interface: Easy to use with intuitive commands
- 🔍 Batch Processing: Process multiple files efficiently
- 📊 Detailed Output: Formatted results with file information

 🚀 Installation

 Prerequisites
- Python 3.7 or higher
- Git (for cloning the repository)

 Steps

1. Clone the repository:
```bash
git clone https://github.com/yourusername/file-hash-calculator.git
cd file-hash-calculator
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

 Alternative: Direct Installation
```bash
pip install tqdm
```

 🛠️ Usage

 Basic Commands

 Calculate Default SHA256 Hash
```bash
python main.py filename.txt
```

 Calculate Specific Algorithm
```bash
python main.py largefile.iso --algorithm sha256
 or
python main.py largefile.iso -a sha256
```

 Calculate All Supported Hashes
```bash
python main.py document.pdf --all
 or
python main.py document.pdf -A
```

 Show Progress Bar (for large files)
```bash
python main.py hugefile.zip --progress
 or
python main.py hugefile.zip -p
```

 Verify Hash Against Expected Value
```bash
python main.py file.zip --verify abc123def456 --algorithm md5
 or
python main.py file.zip -v abc123def456 -a md5
```

 Save Results to File
```bash
python main.py important_file.docx --save results.txt
 or
python main.py important_file.docx -s results.txt
```

 Advanced Usage

 Combined Commands
```bash
 Calculate all hashes with progress bar and save results
python main.py ubuntu-22.04.iso --all --progress --save hash_results.txt
 or
python main.py ubuntu-22.04.iso -A -p -s hash_results.txt
```

 Verify Downloaded File
```bash
 Verify SHA256 hash of a downloaded file
python main.py software_installer.exe --verify "a1b2c3d4e5f6..." --algorithm sha256
```

 📋 Examples

 Example 1: Basic Hash Calculation
```bash
$ python main.py sample.txt

╔════════════════════════════════════════════════════════════════════╗
║                    FILE HASH CALCULATOR                            ║
║                        Cybersecurity Tool                          ║
╚════════════════════════════════════════════════════════════════════╝

📁 File: sample.txt
📊 File Size: 0.02 MB

============================================================
🔐 HASH RESULTS
============================================================
✅ SHA256: b3a8e0e1f9ab1bfe3a36f231f676f78bb30a519d2b21e6c530c0eee8ebb4a5d0
============================================================
```

 Example 2: Hash Verification
```bash
$ python main.py sample.txt --verify "b3a8e0e1f9ab1bfe3a36f231f676f78bb30a519d2b21e6c530c0eee8ebb4a5d0"

╔════════════════════════════════════════════════════════════════════╗
║                    FILE HASH CALCULATOR                            ║
║                        Cybersecurity Tool                          ║
╚════════════════════════════════════════════════════════════════════╝

✅ Hash verification PASSED
```

 Example 3: All Hashes with Progress Bar
```bash
$ python main.py large_file.iso --all --progress

╔════════════════════════════════════════════════════════════════════╗
║                    FILE HASH CALCULATOR                            ║
║                        Cybersecurity Tool                          ║
╚════════════════════════════════════════════════════════════════════╝

🔧 Processing file: large_file.iso
📦 File size: 1024.50 MB

Calculating MD5: 100%|██████████| 1024.5M/1024.5M [00:45<00:00, 22.7MB/s]
Calculating SHA1: 100%|██████████| 1024.5M/1024.5M [00:47<00:00, 21.8MB/s]
Calculating SHA256: 100%|██████████| 1024.5M/1024.5M [00:49<00:00, 20.9MB/s]
Calculating SHA512: 100%|██████████| 1024.5M/1024.5M [01:05<00:00, 15.8MB/s]

============================================================
🔐 HASH RESULTS
============================================================
✅ MD5: d41d8cd98f00b204e9800998ecf8427e
✅ SHA1: da39a3ee5e6b4b0d3255bfef95601890afd80709
✅ SHA256: e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855
✅ SHA512: cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e
============================================================

✓ Results saved to: hash_results.txt
```

 📂 Project Structure
```
file-hash-calculator/
├── src/
│   ├── __init__.py
│   ├── hash_calculator.py     Core hash calculation logic
│   ├── cli.py                Command line interface
│   └── utils.py              Utility functions
├── tests/
│   └── test_hash_calculator.py   Unit tests
├── examples/
│   └── sample_file.txt       Example file for testing
├── requirements.txt          Dependencies
├── main.py                   Main entry point
├── README.md                 This file
└── LICENSE                   License file
```

 🧪 Testing
Untuk menjalankan unit tests:
```bash
python -m unittest discover tests/
```

 🤝 Contributing
Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/new-feature`
3. Commit your changes: `git commit -am 'Add new feature'`
4. Push to the branch: `git push origin feature/new-feature`
5. Open a pull request

 Suggested Improvements
- Add support for more hash algorithms (BLAKE2, SHA3)
- Implement directory scanning capabilities
- Add GUI interface option
- Support for hash comparison between multiple files
- Integration with online hash databases

 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

 🙏 Credits
- Built with ❤️ for cybersecurity professionals and ethical hackers
- Uses Python's built-in `hashlib` library for cryptographic hash functions
- Progress bar powered by `tqdm` library
- Inspired by real-world digital forensics and file integrity verification needs

 📧 Contact
For questions, suggestions, or feedback:
- Create an issue in the GitHub repository
- Email: fazrilfadhilah15@gmail.com

---

🔐 Stay secure, verify your files!  
This tool is designed for legitimate cybersecurity purposes only. Use responsibly and ethically.
