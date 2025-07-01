# Workshop Countdown Dashboard

Live countdown timers and milestone tracking for upcoming workshops.

## Features

- ⏰ Real-time countdown
- 📅 Multiple workshop tracking
- 🎯 Milestone notifications
- 📱 Social sharing widgets
- 📊 Application deadline alerts

## Data Structure

```json
{
  "workshopId": "wog-2025",
  "name": "Workshop on Genomics 2025",
  "startDate": "2025-01-07",
  "endDate": "2025-01-20",
  "applicationDeadline": "2024-10-15",
  "location": "Český Krumlov, Czech Republic",
  "milestones": [
    {
      "date": "2024-10-15",
      "label": "Application Deadline"
    }
  ]
}
```

## Usage

```tsx
import CountdownDashboard from './apps/countdown/CountdownDashboard';

<CountdownDashboard />
```

## WordPress Integration

```html
<div id="evomics-countdown"></div>
<script src="https://shandley.github.io/evomics-web/countdown-embed.js"></script>
```