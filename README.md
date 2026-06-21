# ✈️ Flight Passenger Management System

A C program simulating airport check-in for multiple flights, using custom linked-list-based **queue** and **stack** data structures.

## Features

- Custom singly linked list implementation of:
  - **Queue** (FIFO) — passengers waiting for check-in
  - **Stack** (LIFO) — passengers already boarded
- Flight management with capacity limits
- Check-in workflow: passengers move from the waiting queue to the boarding stack
- Search for a passenger by ID across all flights (queue or stack)
- Recursive printing of queue/stack contents
- Full memory cleanup (no leaks — every `malloc` has a matching `free`)

## Tech Stack

- **C** (standard library only: `stdio.h`, `stdlib.h`, `string.h`)

## How It Works

1. 15 passengers are created and split across 3 flights (Seoul, Rome, Tokyo), 5 per flight, each added to the flight's waiting queue
2. Each flight's queue and stack are printed
3. All waiting passengers are checked in (dequeued → pushed onto the boarding stack)
4. A search is performed for 5 passenger IDs across all flights
5. All allocated memory is freed

## Build & Run

```bash
gcc main.c -o flight_manager
./flight_manager
```

## Author

**Naila** — [@BkNaila](https://github.com/BkNaila)
