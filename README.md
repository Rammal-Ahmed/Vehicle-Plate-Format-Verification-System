# 🚗 Vehicle Number Plate Validator

A small Python command-line tool that checks whether a vehicle number plate is in the correct format. You type a plate, it tells you if it's valid or not. Simple as that.

## How it works

A plate is valid only if it follows this pattern:

| Part | Rule | Example |
|------|------|---------|
| Letters | 3 capital letters | `ABC` |
| Separator | a dash | `-` |
| Digits | 3 numbers | `123` |

Total length is always 7 characters, so `ABC-123` is valid.

## Sample run

```
=============================================
       VEHICLE NUMBER PLATE VALIDATOR
=============================================

Enter Number Plate (e.g. ABC-123) : ABC-123

✔ This vehicle license plate is Valid.

Check another plate? (y/n) : y

Enter Number Plate (e.g. ABC-123) : abc-123

✘ Invalid format. Use 3 capital letters, a dash, then 3 digits.
```

## Valid and invalid examples

| Input | Result | Why |
|-------|--------|-----|
| `ABC-123` | Valid | follows the format |
| `abc-123` | Invalid | letters must be capital |
| `AB-1234` | Invalid | dash is in the wrong place |
| `ABC123` | Invalid | dash is missing |
| `ABC-12A` | Invalid | digits only after the dash |

## Run it

You need Python 3 installed.

```bash
git clone https://github.com/Rammal-Ahmed/vehicle-number-plate-validator.git
cd vehicle-number-plate-validator
python plate_validator.py
```

## What I practiced

- String slicing and indexing
- `isalpha()`, `isupper()` and `isdigit()`
- Writing a reusable function
- Loops and basic input handling

## Ideas for later

- Accept lowercase input automatically
- Show exactly which rule failed
- Support more plate formats
- Add a regex version

## About me

# **Rammal Ahmed**

**AI & Data Science Enthusiast** | **Microsoft Dynamics 365 CRM Developer** | **Power Platform** | **UI/UX Designer** | **Graphic Designer & Illustrator**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rammal-ahmed-58184b325)
[![GitHub](https://img.shields.io/badge/GitHub-Rammal--Ahmed-181717?style=flat&logo=github)](https://github.com/Rammal-Ahmed)

<div align="center">

If you found this useful, consider giving it a star ⭐

**I truly value your feedback and welcome any suggestions for improvement**

**Always open to fresh perspectives, constructive feedback, and new ideas**


## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details

---

*Developed as part of my Python programming practice*

---

**Project Status:** Completed

</div>
