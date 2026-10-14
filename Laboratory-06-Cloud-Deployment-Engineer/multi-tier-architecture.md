# MULTI-TIER ARCHITECTURE OVERVIEW #

## The Web/Application Tier
The web and application tier serves as the front-facing layer of the system. Its primary role is to act as the direct interface for users, handling incoming HTTP requests, rendering the user interface, managing session states, and processing application logic before passing data requests down to the backend.

## The Database Tier
The database tier acts as the backend data management layer. Its core role is to securely store, organize, and retrieve persistent data—such as user credentials, profile information, and file metadata—ensuring that data remains intact and consistent across user sessions.

## Why Separate Them?
Separating the web server and the database into two distinct containers ensures a cleaner separation of concerns, allowing each tier to scale, update, and manage its resource allocation independently. If one tier encounters heavy traffic, a failure, or a security vulnerability, isolation prevents it from crashing or compromising the entire application stack. Furthermore, this modular approach simplifies debugging, maintenance, and future infrastructure upgrades.
