# 🌿 BrightHelp API (Planned)

The BrightHelp API is a planned feature designed to allow approved developers, VA agencies, and partner tools to integrate with the BrightHelp directory, Workspace system, and client–VA matching workflows.

This document outlines the **future direction** of the API, proposed endpoints, and intended functionality.  
As BrightHelp grows, these endpoints will evolve based on user needs and system architecture.

Website: https://brighthelp.ca  
Roadmap: /docs/roadmap.md

---

## ✨ Overview

The future BrightHelp API will focus on:

- retrieving VA directory data (public fields only)  
- submitting client intake requests  
- checking the status of a client match  
- accessing Workspace metadata (not private messages or files)  
- agency-level management tools  
- embedding directory listings into partner websites  
- event-based webhooks for updates  

This API will operate with **strict privacy and permission controls**, prioritizing the confidentiality of both clients and virtual assistants.

---

# 🌱 Planned Authentication

### **🔐 API Key Authentication**
Developers and agency owners will receive:

- a public key  
- a private key  
- permission scopes  

**Scopes may include:**

- `directory.read`  
- `va.profile.read`  
- `client.intake.create`  
- `workspaces.read.metadata`  
- `agency.subcontractors.read`  
- `agency.workspaces.list`  

Authentication will use standard headers:

