<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=DC143C&height=320&section=header&text=Notes%20API&fontSize=96&fontAlignY=38&animation=twinkling&fontColor=ffffff&desc=REST+API+%C2%B7+Node.js+%C2%B7+Express+%C2%B7+MongoDB+%C2%B7+MVC&descAlignY=58&descSize=20&descColor=FFCDD5" />

<br>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=22&duration=2800&pause=900&color=DC143C&center=true&vCenter=true&random=false&width=980&lines=Notes+Management+REST+API+%E2%80%94+Node.js+%2B+Express+%2B+MongoDB;Full+CRUD+%7C+8+Endpoints+%7C+Clean+MVC+Architecture;PUT+vs+PATCH+%7C+Bulk+Create+%7C+Bulk+Delete;Mongoose+Schema+%7C+ObjectId+Validation+%7C+Error+Handling;Backend+Assignment+01+%E2%80%94+CodingGita)](https://github.com/mananjani2102/Notes-App)

<br>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-v18%2B-DC143C?style=for-the-badge&logo=nodedotjs&logoColor=white&labelColor=6B0015" />
  &nbsp;
  <img src="https://img.shields.io/badge/Express-4.x-C41230?style=for-the-badge&logo=express&logoColor=white&labelColor=6B0015" />
  &nbsp;
  <img src="https://img.shields.io/badge/MongoDB-Atlas-A8001E?style=for-the-badge&logo=mongodb&logoColor=white&labelColor=6B0015" />
  &nbsp;
  <img src="https://img.shields.io/badge/Mongoose-ODM-8B0000?style=for-the-badge&logo=mongoose&logoColor=white&labelColor=6B0015" />
  &nbsp;
  <img src="https://img.shields.io/badge/License-MIT-DC143C?style=for-the-badge&logo=opensourceinitiative&logoColor=white&labelColor=6B0015" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Endpoints-8-DC143C?style=flat-square&labelColor=6B0015" />
  &nbsp;
  <img src="https://img.shields.io/badge/Architecture-MVC-C41230?style=flat-square&labelColor=6B0015" />
  &nbsp;
  <img src="https://img.shields.io/badge/Methods-POST%20%7C%20GET%20%7C%20PUT%20%7C%20PATCH%20%7C%20DELETE-A8001E?style=flat-square&labelColor=6B0015" />
  &nbsp;
  <img src="https://img.shields.io/badge/Status-Live-8B0000?style=flat-square&labelColor=6B0015" />
</p>

<br>

<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">

</div>

<br>

<div align="center">

## Live Services

| Service | Platform | URL |
|:-------:|:--------:|:----|
| Backend API | Render | [https://notes-app-1-x5c6.onrender.com](https://notes-app-1-x5c6.onrender.com) |
| Database | MongoDB Atlas | Managed Cloud Cluster |
| API Docs | Postman | _link after publishing_ |

</div>

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## What This API Does

</div>

```
  A clean, minimal Notes Management REST API — no frontend, no authentication.
  Every HTTP method used in real-world production APIs is covered here.

  POST    ->  Create a single note or multiple notes at once (bulk)
  GET     ->  Fetch all notes or retrieve a single note by its ID
  PUT     ->  Full replacement — every field is overwritten with new data
  PATCH   ->  Partial update — only the fields you send are changed
  DELETE  ->  Remove a single note, or wipe multiple notes by an ID array
```

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Tech Stack

<br>

<img src="https://img.shields.io/badge/Node.js-Runtime_Environment-DC143C?style=for-the-badge&logo=nodedotjs&logoColor=white&labelColor=6B0015" />
&nbsp;
<img src="https://img.shields.io/badge/Express-Web_Framework-C41230?style=for-the-badge&logo=express&logoColor=white&labelColor=6B0015" />

<br><br>

<img src="https://img.shields.io/badge/MongoDB-Document_Database-A8001E?style=for-the-badge&logo=mongodb&logoColor=white&labelColor=6B0015" />
&nbsp;
<img src="https://img.shields.io/badge/Mongoose-ODM_Layer-8B0000?style=for-the-badge&logo=mongoose&logoColor=white&labelColor=6B0015" />

<br><br>

<img src="https://img.shields.io/badge/JavaScript-ES6%2B_Language-DC143C?style=for-the-badge&logo=javascript&logoColor=white&labelColor=6B0015" />
&nbsp;
<img src="https://img.shields.io/badge/Postman-API_Testing-C41230?style=for-the-badge&logo=postman&logoColor=white&labelColor=6B0015" />
&nbsp;
<img src="https://img.shields.io/badge/dotenv-Config_Manager-A8001E?style=for-the-badge&logo=dotenv&logoColor=white&labelColor=6B0015" />
&nbsp;
<img src="https://img.shields.io/badge/Nodemon-Dev_Watcher-8B0000?style=for-the-badge&logo=nodemon&logoColor=white&labelColor=6B0015" />

<br><br>

| Layer | Technology | Role |
|:-----:|:----------:|:-----|
| **Server** | Node.js + Express | HTTP server, routing, and JSON middleware |
| **Database** | MongoDB + Mongoose | Document storage with typed schema and validation |
| **Config** | dotenv | Environment variable management for URI and port |
| **Dev** | nodemon | Auto-restart on file changes during development |

</div>

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Project Structure

</div>

```
notes-app/
|
+-- src/
|   +-- config/
|   |   +-- db.js                  <-  mongoose.connect() only
|   |
|   +-- models/
|   |   +-- note.model.js          <-  Mongoose schema + model
|   |
|   +-- controllers/
|   |   +-- note.controller.js     <-  All logic, DB queries, responses
|   |
|   +-- routes/
|   |   +-- note.routes.js         <-  Route definitions only, zero logic
|   |
|   +-- middlewares/               <-  Reserved for future middleware
|   |
|   +-- app.js                     <-  Express setup, json middleware, mount routes
|   +-- index.js                   <-  app.listen() only
|
+-- .env                           <-  Never committed
+-- .env.example                   <-  Committed as reference
+-- package.json
```

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Request Lifecycle

</div>

```
  Incoming HTTP Request
         |
         v
  [ Express Router ]   ->   note.routes.js
         |                  maps URL + HTTP method to a controller function
         v
  [ Controller ]       ->   note.controller.js
         |                  validates input, queries the DB, builds the response
         v
  [ Mongoose Model ]   ->   note.model.js
         |                  enforces schema, validates ObjectId, applies defaults
         v
  [ MongoDB Atlas ]         persists or retrieves documents in the cloud
         |
         v
  [ JSON Response ]         { success, message, data }  sent back to the client
```

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Mongoose Schema

</div>

```js
const noteSchema = new mongoose.Schema(
  {
    title:    { type: String,  required: [true, "Title is required"]   },
    content:  { type: String,  required: [true, "Content is required"] },
    category: { type: String,  enum: ["work", "personal", "study"],
                               default: "personal"                     },
    isPinned: { type: Boolean, default: false                          },
  },
  { timestamps: true }
);
```

<br>

| Field | Type | Required | Details |
|:------|:----:|:--------:|:--------|
| `title` | String | Yes | Cannot be empty |
| `content` | String | Yes | Cannot be empty |
| `category` | String | No | Enum: `work` / `personal` / `study` — Default: `personal` |
| `isPinned` | Boolean | No | Default: `false` |
| `createdAt` | Date | Auto | Generated by `timestamps: true` |
| `updatedAt` | Date | Auto | Generated by `timestamps: true` |

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## API Endpoints

<img src="https://img.shields.io/badge/Base%20URL-%2Fapi%2Fnotes-DC143C?style=for-the-badge&labelColor=6B0015" />

</div>

<br>

| # | Method | Endpoint | Action |
|:-:|:------:|:---------|:-------|
| 1 | ![POST](https://img.shields.io/badge/POST-DC143C?style=flat-square&labelColor=6B0015) | `/api/notes` | Create a single note |
| 2 | ![POST](https://img.shields.io/badge/POST-DC143C?style=flat-square&labelColor=6B0015) | `/api/notes/bulk` | Create multiple notes at once |
| 3 | ![GET](https://img.shields.io/badge/GET-A8001E?style=flat-square&labelColor=6B0015) | `/api/notes` | Retrieve all notes |
| 4 | ![GET](https://img.shields.io/badge/GET-A8001E?style=flat-square&labelColor=6B0015) | `/api/notes/:id` | Retrieve a single note by ID |
| 5 | ![PUT](https://img.shields.io/badge/PUT-C41230?style=flat-square&labelColor=6B0015) | `/api/notes/:id` | Fully replace a note |
| 6 | ![PATCH](https://img.shields.io/badge/PATCH-C41230?style=flat-square&labelColor=6B0015) | `/api/notes/:id` | Partially update a note |
| 7 | ![DELETE](https://img.shields.io/badge/DELETE-8B0000?style=flat-square&labelColor=6B0015) | `/api/notes/:id` | Delete a single note |
| 8 | ![DELETE](https://img.shields.io/badge/DELETE-8B0000?style=flat-square&labelColor=6B0015) | `/api/notes/bulk` | Delete multiple notes by ID array |

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Request & Response Examples

</div>

**POST** `/api/notes` — Create a single note

```json
// Request body
{
  "title": "System Design Notes",
  "content": "Cover load balancing, caching, and sharding.",
  "category": "study",
  "isPinned": true
}

// Response  201 Created
{
  "success": true,
  "message": "Note created successfully",
  "data": {
    "_id": "665f1a2b3c4d5e6f7a8b9c0d",
    "title": "System Design Notes",
    "content": "Cover load balancing, caching, and sharding.",
    "category": "study",
    "isPinned": true,
    "createdAt": "2025-06-04T10:22:14.000Z",
    "updatedAt": "2025-06-04T10:22:14.000Z"
  }
}
```

<br>

**POST** `/api/notes/bulk` — Create multiple notes at once

```json
// Request body
{
  "notes": [
    { "title": "Meeting recap", "content": "Review sprint backlog.", "category": "work"     },
    { "title": "Book list",     "content": "Atomic Habits, DDIA.",   "category": "personal" }
  ]
}

// Response  201 Created
{
  "success": true,
  "message": "2 notes created successfully",
  "data": [ { ... }, { ... } ]
}
```

<br>

**DELETE** `/api/notes/bulk` — Delete multiple notes by ID array

```json
// Request body
{ "ids": ["665f1a2b3c4d5e6f7a8b9c0d", "665f1a2b3c4d5e6f7a8b9c0e"] }

// Response  200 OK
{
  "success": true,
  "message": "2 notes deleted successfully",
  "data": null
}
```

<br>

**Error Responses** — same consistent shape always

```json
// 400 — Invalid ObjectId or missing required field
{ "success": false, "message": "Invalid note ID format", "data": null }

// 404 — Document does not exist
{ "success": false, "message": "Note not found",         "data": null }

// 500 — Unexpected server failure
{ "success": false, "message": "Internal server error",  "data": null }
```

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## PUT vs PATCH

> **The single most important concept in this entire project.**

</div>

<br>

| | `PUT` | `PATCH` |
|:---|:---:|:---:|
| **Strategy** | Full Replacement | Partial Update |
| **Fields not sent** | Reset to defaults | Kept unchanged |
| **Mongoose operator** | Direct assignment | `$set` |
| **Data safety** | Risk of data loss | Safe |
| **Use when** | Replacing entire document | Updating specific fields |

<br>

**Starting document:**
```json
{ "title": "Old title", "content": "Important content", "isPinned": true }
```

<br>

**PUT** — send only `{ "title": "New title" }`
```json
{ "title": "New title", "content": "", "isPinned": false }
```
> `content` and `isPinned` were **wiped to schema defaults** — data lost silently.

<br>

**PATCH** — send only `{ "title": "New title" }`
```json
{ "title": "New title", "content": "Important content", "isPinned": true }
```
> Only `title` changed — **everything else preserved** exactly as it was.

<br>

> Under the hood, PATCH uses Mongoose with `$set` and `{ new: true, runValidators: true }`,
> while PUT reconstructs the full document. Both go through schema validation — only scope differs.

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Response Format

</div>

Every endpoint returns this exact shape — success or error, no exceptions.

```json
{
  "success": true,
  "message": "Human-readable description of what happened",
  "data": { }
}
```

| Field | Type | Value |
|:------|:----:|:------|
| `success` | Boolean | `true` on success, `false` on any failure |
| `message` | String | Always a readable, descriptive string |
| `data` | Object / Array / null | The document, list, or `null` on delete |

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## HTTP Status Codes

</div>

| Code | Meaning | When it fires |
|:----:|:-------:|:--------------|
| ![200](https://img.shields.io/badge/200-OK-DC143C?style=flat-square&labelColor=6B0015) | OK | Successful GET, PUT, PATCH, DELETE |
| ![201](https://img.shields.io/badge/201-Created-C41230?style=flat-square&labelColor=6B0015) | Created | Successful POST — note(s) created |
| ![400](https://img.shields.io/badge/400-Bad_Request-A8001E?style=flat-square&labelColor=6B0015) | Bad Request | Missing fields / invalid ObjectId / empty array |
| ![404](https://img.shields.io/badge/404-Not_Found-8B0000?style=flat-square&labelColor=6B0015) | Not Found | No note exists with the given `_id` |
| ![500](https://img.shields.io/badge/500-Server_Error-6B0015?style=flat-square&labelColor=3D0008) | Server Error | Unexpected database or runtime failure |

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Getting Started

</div>

### 1 — Clone

```bash
git clone https://github.com/mananjani2102/Notes-App.git
cd Notes-App
```

### 2 — Install dependencies

```bash
npm install
```

### 3 — Configure environment

```env
MONGO_URI=your_mongodb_atlas_connection_string
PORT=5000
```

### 4 — Start development server

```bash
npm run dev
```

> Server live at `http://localhost:5000` · MongoDB connected

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Environment Variables

| Variable | Required | Description |
|:---------|:--------:|:------------|
| `MONGO_URI` | Yes | MongoDB Atlas connection string |
| `PORT` | Yes | HTTP port for the Express server |

</div>

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Deployment

<img src="https://img.shields.io/badge/Backend-Render-DC143C?style=for-the-badge&logo=render&logoColor=white&labelColor=6B0015" />
&nbsp;
<img src="https://img.shields.io/badge/Database-MongoDB%20Atlas-A8001E?style=for-the-badge&logo=mongodb&logoColor=white&labelColor=6B0015" />

</div>

<br>

**Backend — Render**

1. Create a Web Service on [render.com](https://render.com) and connect your GitHub repository.
2. Set Build Command to `npm install` and Start Command to `node src/index.js`.
3. Add `MONGO_URI` and `PORT` as environment variables in the Render dashboard.
4. Deploy — live at [https://notes-app-1-x5c6.onrender.com](https://notes-app-1-x5c6.onrender.com)

**Database — MongoDB Atlas**

1. Create a free M0 cluster on [MongoDB Atlas](https://www.mongodb.com/atlas).
2. Create a database user with read/write access.
3. Add `0.0.0.0/0` to the IP allowlist for full Render compatibility.
4. Copy the connection string and set it as `MONGO_URI`.

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

## Scripts

| Script | Command | Description |
|:------:|:-------:|:------------|
| `start` | `node src/index.js` | Production server |
| `dev` | `nodemon src/index.js` | Development with auto-restart |

</div>

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=DC143C&height=4" width="100%">
</div>

<br>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=2500&pause=1000&color=DC143C&center=true&vCenter=true&random=false&width=720&lines=Once+you+understand+PUT+vs+PATCH...;...you+understand+90%25+of+how+REST+APIs+work.)](https://github.com/mananjani2102)

<br><br>

<img src="https://capsule-render.vercel.app/api?type=waving&color=DC143C&height=200&section=footer&text=Clean+REST&fontSize=48&fontAlignY=70&animation=twinkling&fontColor=ffffff" />

</div>
