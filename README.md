# 📊 Discipline & Performance Tracker Pro

A comprehensive, corporate-grade HR analytics dashboard for tracking employee discipline and performance metrics.

![Dashboard Preview](https://img.shields.io/badge/Version-2.0-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![Status](https://img.shields.io/badge/Status-Production%20Ready-success)

## ✨ Features

### 📈 Executive Dashboard
- **KPI Cards**: Total employees, compliance rate, alerts count, average discipline score
- **Real-time Analytics**: Instant calculation of all metrics upon Excel upload
- **Responsive Design**: Works on desktop, tablet, and mobile

### 📊 At-a-Glance Category Cards
- **Outside Office >1Hr**: Track excessive outside time incidents
- **Punch Irregularities**: Monitor bad punches (>6 per day)
- **Leave Applications**: View all leave requests and their status
- **Work From Home**: Track WFH requests and approvals

### 🏆 Performance Tracking
- **Discipline Score (0-100)**: Weighted calculation based on all factors
- **Risk Categories**: Excellent (85+), Good (70-84), Needs Attention (50-69), Critical (<50)
- **Leaderboard**: Top 5 performers
- **Watch List**: Employees needing attention

### 📅 Visual Analytics
- **Trend Charts**: Daily pattern analysis
- **Category Distribution**: Pie chart of risk levels
- **Calendar Heatmap**: Color-coded daily compliance view

### ⚙️ Customization
- **Adjustable Weights**: Configure how each factor affects discipline score
- **Threshold Settings**: Set limits for punches, outside time, WFH, and leaves
- **Dark/Light Mode**: Toggle for comfortable viewing

### 📥 Export Options
- **PDF Export**: Professional reports for meetings
- **CSV Export**: Data for further analysis
- **Print View**: Clean print layout

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended)

1. **Fork this repository** or create a new repo
2. **Upload** `index.html` to your repository
3. Go to **Settings → Pages**
4. Select **Source**: Deploy from a branch
5. Select **Branch**: main, folder: / (root)
6. Click **Save**
7. Access your dashboard at: `https://yourusername.github.io/repo-name/`

### Option 2: Local Use

1. Download `index.html`
2. Open in any modern browser
3. Upload your Excel file
4. Done!

## 📁 Excel File Format

Your Excel file should have these sheets:

### Sheet 1: `OUTSIDE_OFC_>1HRS`
| Column | Description |
|--------|-------------|
| Employee Id | Unique ID (e.g., PR002) |
| Employee Name | Full name |
| Attendance Date | Date of incident |
| Outside Time | Duration (HH:MM:SS) |

### Sheet 2: `PUNCHES`
| Column | Description |
|--------|-------------|
| Employee Id | Unique ID |
| Employee Name | Full name |
| Attendance Date | Date |
| No of Punch | Punch count for the day |

### Sheet 3: `LEAVES`
| Column | Description |
|--------|-------------|
| Employee Id | Unique ID |
| Name | Employee name |
| Designation | Job title |
| Leave Type | FULL DAY / HALF DAY |
| Leave Details | CASUAL LEAVE, etc. |
| From | Start date |
| To | End date |
| Total Days | Number of days |
| Reason | Leave reason |
| Status | APPROVED / PENDING / REJECTED |

### Sheet 4: `WFH`
| Column | Description |
|--------|-------------|
| Department | Department name |
| Employee Id | Unique ID |
| Name | Employee name |
| Designation | Job title |
| From | WFH date |
| To | End date |
| Total Days | Number of days |
| Reason | WFH reason |
| Status | APPROVED / PENDING |

## 📊 Discipline Score Calculation

The discipline score is calculated using weighted factors:

| Factor | Default Weight | Penalty Logic |
|--------|---------------|---------------|
| Outside Office >1Hr | 25% | -5 points per incident (max 25) |
| Bad Punches (>6/day) | 30% | -5 points per bad day (max 30) |
| Leave Frequency | 20% | -3 points per leave day (max 20) |
| WFH Frequency | 25% | -3 points per WFH day over threshold (max 25) |

**All weights and thresholds are adjustable via Settings!**

## 🎨 UI Features

- **Modern Gradient Design**: Contemporary corporate aesthetics
- **Smooth Animations**: Fade-in effects and hover states
- **Interactive Elements**: Click any employee for detailed drill-down
- **Color-Coded Status**: Instant visual feedback on compliance

## 🔒 Privacy & Security

- **100% Client-Side**: No data leaves your browser
- **No Server Required**: All processing happens locally
- **No Data Storage**: Refresh the page and all data is cleared
- **GitHub Pages**: Static hosting, no backend

## 📱 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## 🛠️ Technologies Used

- **HTML5/CSS3**: Modern markup and styling
- **JavaScript (ES6+)**: No frameworks needed
- **SheetJS (XLSX)**: Excel file parsing
- **Chart.js**: Beautiful charts
- **jsPDF**: PDF generation

## 📝 License

MIT License - Feel free to use and modify for your organization.

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

---

**Made with ❤️ for HR Teams**
