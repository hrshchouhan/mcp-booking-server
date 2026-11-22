# mcp-booking-server

mcp-booking-server exposes slot booking as MCP tools (check_availability, book_slot) that AI agents can call on their own. The engineering focus is correctness under concurrency: reproducing race conditions, fixing them with unique constraints, optimistic locking and row-level locks, adding idempotency keys for safe retries, and load-testing with many simulated agents.

Stack: Java 21, Spring Boot, PostgreSQL, Redis, Docker, k6


