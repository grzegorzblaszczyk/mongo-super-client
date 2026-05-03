# Project: Mongo Super Client

This document covers all mandatory features of MongoDB GUI client that must be implemented in vibecoding sessions with Claude Code. 
We focus on features that boost productivity while working with MongoDB server, skipping the enterprise-like features (SSO, advanced auditing etc.)

Features:

## Connection Manager (Security)
* **Goal:** Manage database connections.
* **Features:** Support for connection URIs, SSH Tunneling, SSL/TLS.
* **Vibecode Task:** "Implement a connection secret management module with SSH tunnel support (using `node-ssh`)."

## IntelliShell 
* **Goal:** Editor with auto-complete in real-time.
* **Key features:**
    * Collection and field name autocomplete based on database schema.
    * Support for MongoDB JavaScript methods.
    * Code formatting (Pretty-print).
* **Vibecode Task:** "Integrate the Monaco Editor with a Language Server (LSP) that supports the MongoDB schema."

## Aggregation Editor
* **Goal:** Visually build pipelines stage by stage.
* **Logic:** Each stage has its own input dataset and output preview.
* **Stages to handle:** `$match`, `$group`, `$project`, `$lookup`, `$unwind`.
* **Vibecode Task:** "Build a tab/step system where each aggregation stage is validated and displays a sample of the resulting data."

## Schema Analysis
* **Goal:** Understand data structure in schemaless collections.
* **Features:**
    * Data type detection for fields.
    * Percentage of field occurrence within the collection.
    * Statistical visualization (distribution charts).
* **Vibecode Task:** "Write a script that analyzes a random sample of 1000 documents and generates a report on data types and missing fields."

## Data Import/Export Wizard
* **Goal:** Rapid data migration.
* **Formats:** JSON, CSV, SQL (BSON for backups).
* **Feature:** Mapping CSV columns to MongoDB fields.
* **Vibecode Task:** "Create a streaming CSV importer that allows on-the-fly data type transformations before saving to the database."

## Visual Explain Plan
* **Goal:** Optimize queries and indexes.
* **Logic:** Visual interpretation of the `.explain()` command output.
* **Vibecode Task:** "Process the `explain('executionStats')` result into an operation tree, highlighting full collection scan stages (COLLSCAN) in red."

## Connection Manager (Security)
* **Goal:** Manage database connections.
* **Features:** Support for connection URIs, SSH Tunneling, SSL/TLS.
* **Vibecode Task:** "Implement a connection secret management module with SSH tunnel support (using `node-ssh`)."

