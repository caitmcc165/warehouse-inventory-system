# Warehouse Inventory System

A Python-based inventory and order-management project that demonstrates how core data structures can support common warehouse operations such as stock lookup, inventory updates, FIFO order processing, priority handling, and low-stock reporting.

## What This Project Demonstrates

- Fast inventory lookup using Python dictionaries
- Inventory updates with validation to prevent negative stock
- FIFO order processing with `collections.deque`
- Priority-based task handling with `heapq`
- Low-stock reporting and basic inventory analysis
- Defensive error handling for invalid SKUs, insufficient inventory, and empty queues

## Core Functions

### `lookup_inventory(inventory, sku)`
Returns the current quantity for a SKU and raises a clear error when the SKU does not exist.

### `update_inventory(inventory, sku, quantity_change)`
Adjusts stock for restocking or shipping while preventing inventory from dropping below zero.

### `process_orders(order_queue)`
Processes orders in first-in, first-out order using a queue.

### `process_priority_tasks(priority_queue)`
Retrieves the highest-priority queued task using a heap-based priority queue.

### `generate_inventory_report(inventory, low_stock_threshold)`
Identifies products at or below a configurable low-stock threshold.

## Technologies & Concepts

- Python
- Dictionaries
- Queues / `deque`
- Priority queues / `heapq`
- Data structures and algorithms
- Input validation
- Exception handling
- Inventory and warehouse workflow modeling

## Run Locally

Requires Python 3.

```bash
python warehouse_system.py
