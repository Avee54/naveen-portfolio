# 🎯 **CUSTOMIZATION GUIDE**

## **How to Change Your Company Name & Logo**

### **1. Change Company Name**
In these files, find the `COMPANY_CONFIG` section and change the `name` value:

**Files to edit:**
- `src/components/Header.tsx`
- `src/components/Footer.tsx` 
- `src/app/page.tsx`

**Change this line:**
```tsx
name: "Your Company Name", // ← Change this to your company name
```

**Example:**
```tsx
name: "Acme Solutions", // ← Your actual company name
```

### **2. Add Your Logo**

**Option A: Use an existing logo file**
1. Place your logo image in the `public/` folder
2. Update the `logo` path in the config:

```tsx
logo: "/your-logo.png", // ← Your logo filename
logoAlt: "Acme Solutions Logo", // ← Description of your logo
```

**Option B: Remove logo (text-only)**
```tsx
logo: "", // ← Empty string = no logo
logoAlt: "", // ← Empty string
```

### **3. Change Brand Colors**

**Primary Color Options:**
- `blue` (default)
- `green`
- `purple`
- `red`
- `indigo`
- `teal`
- `pink`
- `yellow`

**Color Intensity Options:**
- `400` (light)
- `500` (medium)
- `600` (default)
- `700` (dark)
- `800` (darker)

**Example - Green theme:**
```tsx
primaryColor: "green", // ← Green theme
accentColor: "600"     // ← Medium-dark green
```

### **4. Quick Customization Example**

Want to change everything to "TechCorp" with a green theme?

```tsx
const COMPANY_CONFIG = {
  name: "TechCorp",           // ← Company name
  logo: "/techcorp-logo.png", // ← Your logo
  logoAlt: "TechCorp Logo",   // ← Logo description
  primaryColor: "green",      // ← Green theme
  accentColor: "600"          // ← Medium green
};
```

### **5. Files That Get Updated Automatically**

✅ **Header** - Company name, logo, colors
✅ **Footer** - Company name, colors  
✅ **Homepage** - Company name in hero and sections
✅ **Navigation** - All pages automatically updated

### **6. Logo Requirements**

- **Format**: PNG, JPG, SVG (recommended)
- **Size**: 40x40px minimum (will scale automatically)
- **Location**: Place in `public/` folder
- **Naming**: Use simple names like `logo.png` or `company-logo.svg`

### **7. After Making Changes**

1. Save the files
2. Your browser will automatically refresh
3. See changes immediately!

---

## **🎨 Need Help?**

- **Company name not changing?** Check all 3 files have the same config
- **Logo not showing?** Make sure the path is correct and file exists in `public/`
- **Colors not updating?** Make sure the color name is valid (blue, green, purple, etc.)

**That's it! Your website will instantly reflect all your changes!** 🚀✨
