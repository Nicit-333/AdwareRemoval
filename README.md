# MacOS Adware Removal Guide  

This repository contains a step-by-step guide for identifying and removing adware, fake notifications, and browser hijacks on macOS Monterey. Designed for both technical users and beginners, the guide combines manual cleanup steps with tool-assisted scans.  

## 📌 Features  

- **Adware Detection** via LaunchAgents, Activity Monitor, and system logs  
- **Safari Hijack Removal** (notifications, extensions, cached data)  
- **Malware Scans** using Malwarebytes and built-in tools  
- **Hardware Diagnostics** to rule out unrelated issues  
- **Prevention Tips** to avoid reinfection  

## 🛠 Requirements  

- **macOS Monterey** (or compatible versions)  
- [Malwarebytes for Mac](https://www.malwarebytes.com/mac) (Free download)  

## 🚀 Removal Instructions  

1. Download Malwarebytes (optional but recommended).  
2. Follow the step-by-step guide in **(AdwareRemoval.md)** to:  
   - Check for suspicious startup items in `~/Library/LaunchAgents` - `~/Library/LaunchDaemons`.  
   - Analyze system logs with `log show` commands.  
   - Clean Safari permissions and website data.  
   - Run Disk Utility and Apple Diagnostics.  

## 📄 Documentation  

Refer to the full guide:  
- **[Detailed Step-by-Step Instructions](AdwareRemoval.md)**  
- **[PDF Version](Removing Adware on macOS.pdf)** (alternative format)  

## 🤝 Contributing  

Found an outdated step or a new adware variant?  
- Open an **issue** to report false positives or missing threats.  
- Submit a **pull request** to improve the guide.  

## 📜 License  

This project is open-source. Feel free to use, modify, and share it.  

## Author  

**Nicolas Cordischi**  

For questions, contact me via [GitHub](https://github.com/Nicit-333) or email.  

## Credits  

This guide was inspired by real-world troubleshooting experiences and community resources like:  
- [Malwarebytes Adware Encyclopedia](https://www.malwarebytes.com/adware)  
- [Apple Support Diagnostics](https://support.apple.com/en-us/HT202731)  
