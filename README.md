# Daily Diary Demo v1 - MVP

## Quick Start

1. **Open the application**:
   - Simply open `index.html` in your web browser
   - Double-click the file, or right-click → Open With → Browser
   - Works in Chrome, Firefox, Safari, Edge

2. **No installation required**:
   - Pure HTML/CSS/JavaScript
   - No dependencies
   - No server needed
   - Data saved in browser localStorage

## Features Implemented

### ✅ 8 Complete Tabs
1. **General** - Contract info, project details, weather, summaries
2. **Personnel** - Staff tracking with auto-calculated totals
3. **Equipment** - Plant and equipment logging
4. **Work Progress** - Activities with planned vs actual tracking
5. **Delays** - Delay causes and hours lost tracking
6. **Safety & Weather** - Incidents, inspections, weather impacts
7. **Production** - Materials, visitors, photos placeholder
8. **Events** - Instructions, variations, cost tracking

### ✅ Core Functionality
- **Dynamic Arrays**: Add/delete rows for personnel, equipment, activities, etc.
- **Dropdowns**: Pre-populated options for standardization
- **Auto-Calculations**: 
  - Personnel totals (staff count, hours, manhours)
  - Activity variances (planned vs actual)
  - Delay totals (hours lost)
- **Digital Signature**: Canvas-based signature capture
- **Data Persistence**: Saves to browser localStorage
- **Entries List**: View all saved diary entries

### ✅ Validation
- Required fields marked with *
- Confirmation checkbox before saving
- Basic field validation

## How to Use

### Creating a New Entry
1. Click **"+ New Entry"** button
2. Fill in tabs sequentially (or jump between tabs)
3. Use **"Add Person"**, **"Add Equipment"**, etc. buttons to add rows
4. Fill in the signature and check the confirmation box
5. Click **"Save Diary Entry"**

### Viewing Entries
1. Click **"Diary Entries"** button
2. See all saved entries with key metrics
3. Delete entries as needed

## MVP 1 Scope

**What's Included:**
- All 8 tabs with core fields from spec
- Dynamic arrays for repeating data
- Auto-calculations and totals
- Basic validation
- localStorage persistence
- Minimal but functional styling

**What's NOT Included (Future Phases):**
- Photo upload (placeholder only)
- Firebase backend
- Advanced validation
- Dashboard for Philip
- Excel export
- Mobile optimization
- Bulk import features

## Technical Details

- **File**: Single HTML file (lean approach)
- **Storage**: Browser localStorage (max ~5-10MB)
- **Data Format**: JSON
- **Browser Support**: All modern browsers
- **Dependencies**: None

## Data Structure

Each diary entry contains:
- Contract & project identification
- Weather conditions (min/max temp, wind, humidity, rainfall)
- Work completed and issues summaries
- Arrays of: personnel, equipment, activities, delays, weather impacts, materials, visitors, events
- Safety information
- Digital signature and confirmation
- Timestamp

## Testing the Demo

### Sample Data Entry Flow:
1. Contract: 24029
2. Supervisor: Willem Jansen van Vuuren
3. Project: SMH/Addax
4. Date: Today
5. Location: Nouakchott, Mauritania
6. Add 2-3 personnel (different roles, hours)
7. Add 1-2 equipment items
8. Add 1 activity (e.g., B20 - Welding, Planned 50%, Actual 35%)
9. Add 1 delay if applicable
10. Fill safety fields
11. Sign and save

## Notes

- Data persists only in the browser where it's created
- Clear browser data will delete all entries
- For production use, implement Firebase backend as per spec
- Photo upload requires backend implementation
- This is a **functional demo** focused on data structure and workflow

## Next Steps (Phase 2+)

1. Backend integration (Firebase)
2. Photo upload functionality
3. Philip's dashboard view
4. Excel export
5. Advanced analytics
6. Mobile app version

---

**Created**: February 2026  
**Version**: MVP 1  
**For**: Philip - Site Management Application
