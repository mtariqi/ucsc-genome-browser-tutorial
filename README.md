# UCSC Genome Browser Custom Track Visualization Tutorial

## Overview
This tutorial demonstrates how to visualize custom genomic data using the UCSC Genome Browser. You'll learn to upload a BED format file and create shareable links for collaborative analysis.

## 📁 Repository Structure

```
ucsc-genome-browser-tutorial/
│
├── README.md                          # This comprehensive tutorial guide
├── test.bed                           # Sample BED file with custom tracks
│
├── data/                              # Sample data files
│   ├── test.bed                       # Original BED file (chr22 tracks)
│   └── examples/                      # Additional example files
│       ├── example_simple.bed         # Minimal BED example
│       ├── example_colored.bed        # Multi-track colored example
│       └── example_genes.bed          # Gene annotation example
│
├── screenshots/                       # Visual guides
│   ├── 01_gateway.png                 # UCSC Gateway page
│   ├── 02_add_custom_tracks.png       # Add custom tracks button
│   ├── 03_upload_file.png             # File upload interface
│   ├── 04_track_display.png           # Browser view with tracks
│   ├── 05_my_sessions.png             # Sessions menu
│   ├── 06_save_session.png            # Save session dialog
│   └── 07_share_link.png              # Generated shareable link
│
├── docs/                              # Additional documentation
│   ├── bed_format_guide.md            # Detailed BED format specifications
│   ├── troubleshooting.md             # Extended troubleshooting guide
│   ├── advanced_features.md           # Advanced UCSC Browser features
│   └── faq.md                         # Frequently asked questions
│
├── scripts/                           # Utility scripts
│   ├── validate_bed.py                # Python script to validate BED files
│   ├── convert_coordinates.py         # Coordinate conversion (hg19↔hg38)
│   ├── generate_bed.py                # Generate sample BED files
│   └── README.md                      # Scripts documentation
│
├── examples/                          # Complete example workflows
│   ├── basic_workflow/
│   │   ├── README.md                  # Basic workflow tutorial
│   │   ├── input.bed                  # Input data
│   │   └── session_link.txt           # Resulting session link
│   │
│   ├── multiple_tracks/
│   │   ├── README.md                  # Multiple tracks tutorial
│   │   ├── track1.bed                 # First track
│   │   ├── track2.bed                 # Second track
│   │   └── combined.bed               # Combined tracks file
│   │
│   └── annotation_project/
│       ├── README.md                  # Annotation project example
│       ├── genes.bed                  # Gene annotations
│       ├── variants.bed               # Variant positions
│       └── regulatory.bed             # Regulatory elements
│
├── templates/                         # BED file templates
│   ├── template_basic.bed             # Basic track template
│   ├── template_scored.bed            # Scored features template
│   ├── template_colored.bed           # Colored tracks template
│   └── README.md                      # Template usage guide
│
├── .gitignore                         # Git ignore file
├── LICENSE                            # License information
└── CONTRIBUTING.md                    # Contribution guidelines
```

## 📄 File Descriptions

### Root Directory
- **README.md**: Main tutorial and comprehensive guide (this file)
- **test.bed**: Primary sample BED file used in the tutorial with two custom tracks

### `/data` Directory
Contains all sample data files used in tutorials and examples:
- **test.bed**: Copy of the main sample file
- **examples/**: Additional BED file examples for different use cases
  - Simple single-track examples
  - Multi-track colored visualizations
  - Gene annotation examples

### `/screenshots` Directory
Visual guides showing each step of the tutorial:
- Sequential numbered screenshots (01-07)
- Shows UCSC interface at each step
- Helps users verify they're following correctly
- Useful for troubleshooting

### `/docs` Directory
Extended documentation and guides:
- **bed_format_guide.md**: In-depth BED format specifications (3-12 column formats)
- **troubleshooting.md**: Common issues and solutions
- **advanced_features.md**: Track hubs, bigBed, custom colors, etc.
- **faq.md**: Answers to frequently asked questions

### `/scripts` Directory
Python utilities for working with BED files:
- **validate_bed.py**: Check BED file format validity
- **convert_coordinates.py**: Convert between genome assemblies (liftOver)
- **generate_bed.py**: Create sample BED files for testing
- Each script includes usage examples and documentation

### `/examples` Directory
Complete workflow examples with step-by-step instructions:
- **basic_workflow/**: Single track upload example
- **multiple_tracks/**: Working with multiple simultaneous tracks
- **annotation_project/**: Real-world genomic annotation example

### `/templates` Directory
Ready-to-use BED file templates:
- Various template formats for different needs
- Copy, modify, and use for your own data
- Includes usage instructions

## 🎯 Quick Start Files

For the assignment, you only need:
- ✅ `README.md` (main tutorial)
- ✅ `test.bed` (sample data)

## 📊 Minimal vs Complete Repository

### Minimal Repository (Assignment)
```
ucsc-tutorial/
├── README.md
└── test.bed
```

### Complete Repository (Full Tutorial)
All directories and files listed above for comprehensive learning resource.

## About the Data
The `test.bed` file contains two custom tracks:
- **Spacer track**: Blue markers at 10kb intervals (chr22:20,100,000-20,140,000)
- **Even track**: Red markers at specific 100bp intervals with labels

## Prerequisites
- Web browser with internet connection
- The `test.bed` file from this repository
- (Optional) Free UCSC Genome Browser account for saving sessions

---

## Step-by-Step Instructions

### Step 1: Access the UCSC Genome Browser

1. Navigate to [UCSC Genome Browser Gateway](https://genome.ucsc.edu/cgi-bin/hgGateway)
2. Select genome assembly: **Human GRCh38/hg38** (or GRCh37/hg19)
3. In the position/search box, you can enter: `chr22:20,100,000-20,140,000`

### Step 2: Add Custom Track - Method A (Upload File)

1. Click the **"add custom tracks"** button on the Gateway page
2. On the "Manage Custom Tracks" page, click **"Choose File"** or **"Browse"**
3. Select the `test.bed` file from this repository
4. Click **"Submit"**
5. Review the confirmation page showing your loaded tracks
6. Click **"go to genome browser"** to visualize the data

### Step 2: Add Custom Track - Method B (Paste Data)

Alternatively, you can paste the data directly:

1. Click **"add custom tracks"** on the Gateway page
2. Copy the entire contents of `test.bed`
3. Paste into the text box on the "Manage Custom Tracks" page
4. Click **"Submit"**
5. Click **"go to genome browser"**

### Step 3: Verify Track Display

You should see two custom tracks in the browser:

| Track Name | Color | Description |
|------------|-------|-------------|
| spacer | Blue (RGB: 0,0,255) | Three tick marks at 10kb intervals |
| even | Red (RGB: 255,0,0) | Three tick marks with labels (first, second, third) |

**Troubleshooting**: If tracks don't appear:
- Right-click on track labels and select visibility mode: **"full"** or **"dense"**
- Check that you're viewing the correct region: chr22:20,100,000-20,140,000
- Verify the genome assembly matches (hg38 or hg19)

### Step 4: Create Shareable Link - Using Sessions (Recommended)

This method creates a permanent, easy-to-share link:

1. From the browser view, click **"My Data"** → **"My Sessions"** in the top blue menu
2. Click **"Save Settings"**
3. If not logged in, you'll be prompted to create a free account or log in
4. Fill in the session details:
   - **Session Name**: e.g., "Chr22 Custom Tracks Demo"
   - **Description**: (optional) Brief description of your data
   - ✅ Check **"allow this session to be loaded by others"**
5. Click **"Submit"**
6. Copy the generated session URL (format: `https://genome.ucsc.edu/s/username/sessionname`)

**Advantages of Sessions**:
- Short, memorable URLs
- Includes all browser settings and custom tracks
- Can be updated without changing the URL
- More reliable for sharing

### Step 5: Create Shareable Link - Using URL Parameters (Alternative)

Quick method without creating an account:

1. After loading your custom tracks, click **"View"** → **"In Other Browsers (custom tracks)"**
2. Copy the generated URL from the pop-up window

**Note**: URLs with embedded custom data can be very long and may have limitations.

### Step 6: Test Your Shareable Link

Important validation step:

1. Open a **new private/incognito browser window**
2. Paste your shareable link
3. Verify that:
   - The browser loads to the correct position (chr22:20,100,000-20,140,000)
   - Both custom tracks are visible
   - Track colors are correct (blue and red)
   - Labels appear on the "even" track

### Step 7: Share Your Link

Use your tested link for:
- Assignment submissions
- Collaboration with colleagues
- Documentation in publications
- GitHub repository documentation

---

## Understanding BED Format

The `test.bed` file uses UCSC BED format with track definition lines:

```
track name=TrackName description="Description" color=R,G,B
chr  start  end  [label]
```

### Example from test.bed:
```
track name=spacer description="Blue ticks every 10000 bases" color=0,0,255
chr22   20100000 20100001
chr22   20110000 20110001
chr22   20120000 20120001
```

**Key Points**:
- Coordinates are 0-based, half-open (start inclusive, end exclusive)
- Colors are RGB values (0-255 for each channel)
- Optional 4th column for feature labels
- Track lines define display properties

---

## Additional Resources

### UCSC Genome Browser Documentation
- [Custom Track Documentation](https://genome.ucsc.edu/goldenPath/help/customTrack.html)
- [BED Format Specification](https://genome.ucsc.edu/FAQ/FAQformat.html#format1)
- [Sharing Data with Sessions and URLs](https://genome-blog.gi.ucsc.edu/blog/2021/08/13/sharing-data-with-sessions-and-urls/)
- [FAQ: Linking to the Genome Browser](https://genome.ucsc.edu/FAQ/FAQlink.html)

### Tips for Custom Tracks
- **File size limits**: Custom tracks via URL have size limitations; use Track Hubs for large datasets
- **Track visibility**: Right-click track names to adjust display modes (hide/dense/squish/pack/full)
- **Color coding**: Use RGB values to distinguish different track types
- **Session management**: Sessions inactive for 4+ months are automatically deleted
- **Browser compatibility**: Works best with Chrome, Firefox, and Safari

---

## Troubleshooting

### Problem: Tracks don't appear after upload
**Solution**: 
- Check track visibility settings (right-click on track label)
- Verify you're viewing the correct genomic region
- Ensure chromosome names match (chr22 vs 22)

### Problem: Shareable link doesn't work
**Solution**:
- Test in incognito/private window
- For long URLs, use Session method instead
- Verify "allow others to load" is checked for sessions

### Problem: Wrong genome assembly
**Solution**:
- Confirm your BED file chromosome names match the assembly
- Use hg38 (GRCh38) for current human genome
- Convert coordinates if necessary using liftOver tool

---

## License
This tutorial and sample data are provided for educational purposes.

## Contributing
Feel free to submit issues or pull requests to improve this tutorial.

## Contact
For questions about UCSC Genome Browser, visit their [help page](https://genome.ucsc.edu/contacts.html).

---

## Quick Reference Commands

### View the custom track directly (copy and paste this URL):
```
https://genome.ucsc.edu/cgi-bin/hgTracks?db=hg38&position=chr22:20100000-20140000
```
Then add your custom track using the "add custom tracks" button.

---

**Last Updated**: October 2025
