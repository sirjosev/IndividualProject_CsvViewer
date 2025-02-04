## Usage

### Command Line Version
```bash
python csv_to_table.py input.csv
```

### Google Colab Version
1. Upload your CSV when prompted
2. Get instant formatted table output

## Use Cases & Applications

### 🔍 Data Reporting
- Convert raw survey data into presentable formats
- Create quick reports from analytics exports

### 🛠️ CLI Utilities
- Integrate with shell scripts for automated reporting
- Combine with cron jobs for daily data summaries

### 🎓 Education
- Format student grade data
- Create assignment solution templates

### 💾 Data Migration
- Visualize CSV data before database import
- Validate data structure during ETL processes

### 🐛 Debugging
- Inspect CSV contents during data processing
- Verify data cleaning results

## Benefits

✅ **Automation Friendly** - Easy to integrate into data pipelines  
✅ **Human Readable** - Better than raw CSV for quick inspections  
✅ **No Dependencies** - Pure Python implementation  
✅ **Cross-Platform** - Works on Windows/Linux/Mac and Colab  

## Example

**Input CSV**:
```csv
Name,Age,City
Andi,25,Jakarta
Budi,30,Bandung
```

**Output**:
```
-------------------------------------
| No  | Name   | Age  | City      |
-------------------------------------
| 1   | Andi   | 25   | Jakarta   |
-------------------------------------
| 2   | Budi   | 30   | Bandung   |
-------------------------------------
```

## Customization

Modify these parts of the code for different use cases:

1. **Different Delimiters**:
```python
# Change CSV dialect
pembaca = csv.reader(csvfile, delimiter=';')
```

2. **Alternative Styles**:
```python
# Modify table borders
contoh_baris = "+" + "+".join(f"{'-'*lebar[i]}" for i in range(len(header))) + "+"
```

3. **Additional Formatting**:
```python
# Add color codes for terminal output
baris_str = "\033[92m|\033[0m" + "\033[93m|\033[0m".join(...)
```

## Contribution

Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## License

MIT License - Free for commercial and personal use

---

**Adaptation Guide**:
- For tab-separated files: Modify delimiter in csv.reader
- For huge files: Implement batch processing
- For HTML output: Modify the string formatting section
