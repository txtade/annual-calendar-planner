# Annual Calendar Planner

A custom-built interactive annual planner with a horizontal timeline/gantt-style view. Multi-day color-coded event bars, drag-to-create, and a single-file architecture that runs in any browser.

Inspired by [app.anucal.com](https://app.anucal.com). Built January 2026.

## What's in this repo

### Active files

- **annual-planner-v6.html** -- General annual planner for life/business planning. Standalone HTML with hybrid save.
- **cookingchew-pin-calendar-synced.html** -- Pinterest pin calendar for CookingChew. Google Sheets synced version with pinterest-specific categories and two-phase burst timing.
- **CookingChew_Master_Seasonal_Two_Phase_Pinning_2026.csv** -- Master data source for seasonal pin burst dates. 23 seasonal moments with ahead-start, ahead-end, close-start, and close-end windows.

### Archive

Old versions kept for reference:

- annual-planner-v5.html
- cookingchew-pin-calendar-2026-non-synced.html
- Pinterest-Ready-Version-pin-calendar-2026.html
- cookingchew-pin-calendar-synced-redownload-feb25.html

## Features

- Horizontal timeline with months as rows, days as columns
- Click + drag across days to create multi-day event bars
- "Add Event" button with form (dropdowns for month, start day, end day) as alternative to drag
- Events can span across months
- Click any event bar to edit title, dates, category, or delete
- Duplicate event button for repeating items
- Notes field on events (events with notes get a white left border, hover for tooltip)
- 19 color options for categories
- US holidays overlay with red dots (toggle on/off)
- Custom category management via gear icon
- Default categories: travel, content, newsletter, social, personal, seasonal, other

## Save system

Hybrid save architecture:

- **Auto-save** to localStorage runs in background during a session (safety net)
- **Save File button** exports a new HTML file with all data baked in (the real save)
- Single-file system: one HTML file contains both the app and your data
- No separate JSON file needed

Workflow: open HTML > make changes > hit Save File > replace old file in iCloud/Google Drive.

**Save before** closing the tab, switching devices, or clearing browser cache.

## Printing

- Split print mode: toggle between Full, 2-Page, and 3-Page in the toolbar
- 2-Page splits at day 15
- 3-Page gives a wider layout with holiday names visible
- Events spanning both halves show on both pages

## Works on

- Mac (any browser)
- iPad (Safari)
- Printable to PDF

## License

Private tool. Not for distribution.
