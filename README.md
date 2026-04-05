# Shift Schedule Planner

A browser-based workforce scheduling tool designed to support fast shift planning, staffing simulation, and day-by-day schedule generation.

## Problem

Shift planning in operations teams is often handled manually in spreadsheets. This creates several common problems:

- Scheduling takes time and is difficult to adjust quickly
- Staffing balance across days and shifts is hard to control
- Comparing planned staffing against target ratios is tedious
- Running "what-if" scenarios requires repeated manual edits

This project was built to reduce that friction by providing a lightweight scheduling tool that runs directly in the browser.

## Solution

Shift Schedule Planner helps generate a weekly schedule based on configurable workforce rules such as:

- total number of employees
- working hours
- days off
- enabled shifts
- staffing ratios by day
- staffing ratios by shift
- shift distribution targets

The goal is not to replace enterprise workforce management platforms, but to provide a practical front-end utility for quick planning, simulation, and internal staffing experiments.

## Key Features

- Configure total employees, work hours, and days off
- Enable or disable up to 8 shifts
- Define staffing ratios by day of week
- Define staffing ratios by shift
- Generate a weekly shift schedule automatically
- View daily staffing summary against target ratios
- Export schedules to Excel
- Save and load configuration in the browser

## Use Cases

- Contact center workforce planning
- Operations staffing simulation
- Internal shift design and testing
- Quick "what-if" scenario analysis before final scheduling

## Scheduling Logic

The planner uses configurable rules to distribute staffing across the week and across enabled shifts.

At a high level, the workflow is:

1. Define workforce size and shift structure
2. Set daily staffing ratios
3. Set per-shift distribution targets
4. Generate a weekly allocation based on those rules
5. Compare generated staffing with expected targets

This makes it easier to test scheduling assumptions before moving to final operational planning.

## Tech Stack

- HTML
- CSS
- JavaScript
- SheetJS (XLSX) for Excel export

## Run Locally

This is a lightweight static front-end application.

### Option 1: Open directly
1. Clone or download this repository
2. Open `index.html` in your browser

### Option 2: Run with a local server
If you prefer, run it with a simple local server for easier testing.

## Why This Project Matters

This project reflects a practical approach to workforce planning: instead of treating scheduling as a purely manual task, it turns planning logic into a usable browser-based tool that supports faster decision-making.

It is especially useful in environments where teams need quick schedule generation, staffing experiments, or planning support without relying on a full backend system.

## Current Scope and Limitations

This project is intentionally lightweight.

Current limitations include:

- no backend or database
- no employee preference handling
- no advanced fairness optimization
- no complex rule engine for enterprise-grade rostering

It is best positioned as a fast planning and simulation utility, not a full workforce management platform.

## Future Improvements

Possible next steps include:

- employee-level preference rules
- fairness balancing across shifts
- stronger constraint handling
- role/skill-based assignment
- improved visualization and reporting
- optional backend integration for persistence and team usage
