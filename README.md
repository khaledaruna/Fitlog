# FitLog 

### Workout Library & Personal Training Planner

FitLog is a responsive workout library and
daily workout planning application.

[**Live Demo**](https://fitlog-seven-beta.vercel.app) · 

[**Source Code**](https://github.com/khaledaruna/fitlog)


## About FitLog

**FitLog** is a workout library and personal training planner built around a simple workflow:

**discover → review → plan → complete**

Users can explore workouts, open detailed exercise guides, build a daily routine, save workouts for later, track workout totals, and keep their selections available across page refreshes.

The interface follows a focused dark fitness aesthetic and is fully responsive across mobile, tablet, and desktop devices.

---

## What You Can Do

** Feature/Structure

```text

├── **Phase 1
│   ├── Next.js setup
│   ├── Tailwind
│   ├── DaisyUi
|   ├── Lucide
│   ├── Sonner
│   │
├── **Phase 2
│   ├── Layout
│   ├── Navbar
│   ├── Footer
|   ├── Lucide
│
├── **Phase 3
│   ├── Api
│   ├── Typescript type
│   ├── home
|   ├── Loading
│  
│
├── **Phase 4
│   ├── Without Card
│   ├── Library
│   ├── sort
│
├── **Phase 5
│   ├── Dynamic Route
│   ├── Details
│   ├── Specs
|   ├── Instructions
│
├── **Phase 6
│   ├── Context
│   ├── Today's Plan
│   ├── Saved
|   ├── Counters
│  
│
├── **Phase 7
│   ├── Toast
│   ├── Remove
│   ├── Mark Done
│   ├── LocalStorage
│  
│
├── **Phase 8
│   ├── 404
│   ├── Respon sive
│   ├── README
│   ├── Deployment
│
```
---
## Core Experience

### Workout Library

The main library presents all available workouts in a responsive card layout.

Each workout includes:

- Exercise image
- Muscle group tags
- Workout name
- Required equipment
- Duration
- Calories burned
- Rating

A live search field allows users to quickly filter workouts by **name** or **muscle group**.

### Workout Details

Every workout has its own dynamic details page with:

- Description
- Target muscle groups
- Equipment
- Difficulty
- Sets and repetitions
- Duration
- Calories
- Rating
- Step-by-step instructions

From the details page, a workout can be added to **Today's Plan** or **Saved for Later**.

### Today's Plan

Today's Plan is built for focused daily training.

Users can:

- Add up to **5 workouts**
- View live workout totals
- Sort the current plan
- Mark exercises as done
- Open workout details
- Remove exercises from the plan

Once five workouts have been added, the plan is locked until an existing workout is removed.

### Saved Workouts

The Saved section acts as a personal exercise collection.

Users can:

- Save workouts independently from Today's Plan
- Store multiple workouts without a daily limit
- Sort saved exercises
- Open workout details
- Remove saved workouts
- View statistics for the active collection

---

## Thoughtful UX

FitLog includes a number of smaller details that make the overall experience feel complete:

- Active navigation states
- Live Plan and Saved counters
- Duplicate workout prevention
- Disabled states for already-added workouts
- Five-workout plan limit
- Completed workout states
- Toast notifications
- Search empty state
- Plan and Saved empty states
- Loading indicators and skeletons
- Custom error interface
- Custom 404 page
- Smooth scroll behavior
- Scroll-to-top control
- Persistent client state

---

## Tech Stack

| Technology          | Role                                          |
| ------------------- | --------------------------------------------- |
| **Next.js 16**      | App Router, rendering, routing, data fetching |
| **React 19**        | Component architecture and interactivity      |
| **TypeScript**      | Type-safe application development             |
| **Tailwind CSS 4**  | Responsive styling                            |
| **DaisyUI**         | Tailwind utility components                   |
| **Lucide React**    | Interface icons                               |
| **React Hot Toast** | Action feedback and notifications             |
| **Local Storage**   | Persistent workout state                      |
| **Vercel**          | Deployment                                    |

---

## Routes

| Route                | Description                |
| -------------------- | -------------------------- |
| `/`                  | Workout library            |
| `/workouts/[id]`     | Individual workout details |
| `/my-plan?tab=plan`  | Today's Plan               |
| `/my-plan?tab=saved` | Saved Workouts             |

Invalid routes and unavailable workout IDs are handled through a dedicated Not Found experience.


## Data Source

Workout data is loaded from the FitLog API.

**All workouts**

```text
https://api.abcz.workers.dev/api/fitlog
```

**Single workout**

```text
https://api.abcz.workers.dev/api/fitlog/:id
```

---

## State Management

Workout state is managed through React Context and persisted in Local Storage.

The application keeps track of:

```text
plan
saved
completedIds
```

This allows users to refresh or revisit the app without losing their current workout selections.

---

## Run Locally

Clone the repository:

```bash
git clone https://github.com/khaledaruna/fitlog.git
```

Enter the project:

```bash
cd fitlog
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open:

```text
http://localhost:3000
```

---

## Scripts

| Command         | Purpose                      |
| --------------- | ---------------------------- |
| `npm run dev`   | Start the development server |
| `npm run lint`  | Run ESLint                   |
| `npm run build` | Create a production build    |
| `npm run start` | Run the production build     |

---

## Responsive Layout

| Device      | Experience                                   |
| ----------- | -------------------------------------------- |
| **Mobile**  | Single-column, touch-friendly layout         |
| **Tablet**  | Balanced multi-column interface              |
| **Desktop** | Expanded workout grid and planning dashboard |


<div>

### Train with intent. Log every set.

[**Open FitLog →**](https://fitlog-seven-beta.vercel.app/)

</div>