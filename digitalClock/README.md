# PyQt5 Digital Clock

This is a simple **digital clock** built using **PyQt5**. It displays the current time and updates every second.  
The clock features a **custom font**, **customizable size**, and **color scheme**.

## Requirements

To run this script, you need to install **PyQt5**:

```bash
pip install PyQt5
```

Then, run the script using:

```bash
python digital_clock.py
```

The digital clock will open in a **resizable window**, and the time updates every second.

---

## Customization  

### Change Font

By default, the script uses the font `"DS-DIGIT.TTF"`.  
If you want to change the font, follow these steps:

1. Download a **.TTF** font file of your choice.
2. Place the font file in the **project folder**.
3. Open `digital_clock.py` and modify the following line (**Line 27**):

   ```python
   font_id = QFontDatabase.addApplicationFont("path/to/your-font.ttf")
   ```

4. Also, update **Line 28** to apply the new font:

   ```python
   font_family = QFontDatabase.applicationFontFamilies(font_id)[0]
   ```

---

### Change Font Size

The font size is defined in **Line 29**:

```python
my_font = QFont(font_family, 150)  
```

- Increase the number for **larger text**.
- Decrease the number for **smaller text**.

---

### Change Font Color

The font color is set in **Line 22**:

```python
self.time_label.setStyleSheet("font-size: 150px; color: hsl(272, 61%, 60%);")
```

Modify `"hsl(272, 61%, 60%)"` to another **HSL** or **Hex** color:  
- **HSL Example**: `hsl(0, 100%, 50%)` (Red)  
- **Hex Example**: `#FF5733` (Orange)

---

### Change Background Color

The background color is defined in **Line 23**:

```python
self.setStyleSheet("background-color: darkgray;")
```

Replace `"darkgray"` with any **color name**, **hex code**, or **HSL value**.



