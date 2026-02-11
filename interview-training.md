# Calendar Exercise

You are given a list of calendar events.
Each event has:
• a title
• a start time (ISO string)
• an end time (ISO string)

Some events overlap in time and should be merged into a single event block.

Your task is to normalize the schedule by merging overlapping events and returning them in chronological order.

```ts
type Event = {
  title: string;
  start: string; // ISO date-time
  end: string; // ISO date-time
};

function normalizeSchedule(events: Event[]): Event[] {
  // ...
}
```

Example input:

```ts
[
  {
    title: "Daily Standup",
    start: "2026-01-10T09:00",
    end: "2026-01-10T09:30",
  },
  {
    title: "Planning",
    start: "2026-01-10T09:15",
    end: "2026-01-10T10:00",
  },
  {
    title: "Lunch",
    start: "2026-01-10T12:00",
    end: "2026-01-10T13:00",
  },
];
```
