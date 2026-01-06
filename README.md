# Meeting Coordination System

⚠️ **DEPRECATED PROJECT** - No longer maintained

## About

This repository contains archived code from a location tracking and meeting coordination system developed in 2025. The project was used for secure meeting point planning and coordinate management.

**Status:** 🔴 Archived (Last updated: August 2024)

---

## ⚠️ WARNING

This repository was accidentally left public and contains sensitive configuration data that should have been removed. It includes:

- Geographic coordinates
- API credentials (expired)
- Database connection strings
- Meeting location data
- Configuration files with hardcoded values

**This is not a security best practice. Do NOT use this code in production.**

---


## Files Description

### `config.py`
Configuration file containing:
- API keys for mapping services (Google Maps, Mapbox)
- Database credentials
- Meeting location coordinates
- Time and date settings
- Security settings (outdated)

⚠️ **Contains hardcoded credentials - DO NOT USE**

### `Meeting.txt`
Plain text file with:
- Primary meeting point coordinates
- Backup location coordinates  
- Meeting time and date
- Access codes and security protocols


## Data Format

### Coordinates Format
Coordinates are stored in decimal degrees format:
```
Latitude: XX.XXXXX (North)
Longitude: XX.XXXXX (East)
```

### Date/Time Format
```
Date: YYYY-MM-DD
Time: HH:MM (24-hour format)
Timezone: Asia/Almaty (GMT+6)
```

---

## Usage (Historical)

This system was designed to:
1. Store and manage meeting location coordinates
2. Provide backup location data
3. Encode sensitive geographic information
4. Facilitate secure meeting coordination

**Example workflow:**
```python
from config import get_coordinates

# Get meeting coordinates
lat, lon = get_coordinates()
print(f"Meeting at: {lat}, {lon}")
```

---

## Security Issues

### Known Vulnerabilities ⚠️

1. **Exposed API Keys**
   - Google Maps API key in plaintext
   - Mapbox token not rotated
   - Database passwords hardcoded

2. **No Encryption**
   - Coordinates stored in plaintext
   - Configuration files not encrypted
   - No use of environment variables

3. **Public Repository**
   - Sensitive data committed to public repo
   - .gitignore added after sensitive commits
   - Commit history contains credentials

4. **Hardcoded Values**
   - Database connection strings
   - API endpoints
   - Meeting locations and times

---

## Why This Repository Exists

This is an **archived educational example** of what NOT to do with sensitive data:

❌ Don't commit API keys to repositories  
❌ Don't store passwords in code  
❌ Don't hardcode coordinates and sensitive data  
❌ Don't leave public repos with confidential info  
❌ Don't forget to use .env files  

✅ Use environment variables  
✅ Encrypt sensitive data  
✅ Use secret management tools  
✅ Follow security best practices  
✅ Rotate credentials regularly  

---

## Technologies Used

- **Python 3.8+** - Core language
- **JSON** - Data storage format
- **Base64** - Basic encoding (not encryption!)
- **PostgreSQL** - Database (credentials exposed)

---

## Installation (Don't Actually Do This)

```bash
# Clone the repository
git clone https://github.com/KINGSPOONKIBAB/shadowtrade-coords.git

# Install dependencies (there are none because I'm bad at this)
cd shadowtrade-coords

# Run configuration
python config.py

# ⚠️ WARNING: This will expose all credentials
```

---

## Contributing

This project is **ARCHIVED** and no longer accepts contributions.

If you found this repository and noticed the security issues - yes, I know. It's too late now.

---

## License

This project has no license because it shouldn't exist in the first place.

Use at your own risk. Actually, don't use it at all.

---

## Contact

For security concerns: ~~Don't bother, damage is done~~

GitHub: [@KINGSPOONKIBAB](https://github.com/KINGSPOONKIBAB)

---

## Lessons Learned

1. Always use `.gitignore` BEFORE committing
2. Never commit sensitive data
3. Use environment variables for credentials
4. Rotate API keys regularly
5. Don't be like me

---

## Changelog

### v1.2.0 (2023-08-15) - Final Update
- Added coordinates for primary meeting location
- Updated configuration with API keys (oops)
- "Fixed" database connection strings (made worse)
- Added this README (too little, too late)

### v1.1.0 (2023-07-20)
- Initial configuration setup
- Added location data structures
- Committed credentials by mistake

### v1.0.0 (2023-07-15)
- Project initialization
- Basic structure created

---

## FAQ

**Q: Why are API keys exposed in this repo?**  
A: Mistakes were made.

**Q: Should I use this code?**  
A: Absolutely not.

**Q: Can I fork this project?**  
A: You can, but why would you?

**Q: Is this data real?**  
A: 🤷 That's for you to find out.

**Q: Where are the coordinates pointing to?**  
A: Check the files. It's all there. Unfortunately.

---

## Disclaimer

This repository is archived and contains historical data from 2023. All API keys should be considered compromised. Database credentials are expired. Meeting locations may no longer be relevant.

**DO NOT USE THIS CODE IN ANY PRODUCTION ENVIRONMENT.**

This is a cautionary tale about poor security practices.

---

## Acknowledgments

Thanks to:
- Nobody, because this is embarrassing
- My past self for being careless
- GitHub for hosting my mistakes forever

---

**Last Updated:** August 15, 2024  
**Status:** Deprecated / Abandoned  
**Security Level:** 💀 Compromised

---
