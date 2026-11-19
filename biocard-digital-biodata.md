# Portfolio Project Data — BioCard - Digital Biodata

- **Category:** `desktop-mobile` (Mobile App)
- **Category Label:** `Mobile App`
- **Accent Color:** `amber`
- **Target Assets Folder:** `public/images/projects/biocard_digital_biodata/`
- **Required Local Images:** `banner.webp`, `image01.webp` .. `image03.webp`

## TypeScript Data (`ProjectCaseStudy`)

```typescript
{
  "id": "biocard-digital-biodata",
  "code": "PRO-22 // APP-01",
  "title": "BioCard - Digital Biodata",
  "category": "desktop-mobile",
  "categoryLabel": "Mobile App",
  "year": "2022",
  "status": "Completed",
  "accentColor": "amber",
  "repoUrl": "https://github.com/weztcy/BioCard---Digital-Biodata",
  "license": "MIT License",
  "imageUrl": "/images/projects/biocard_digital_biodata/banner.webp",
  "images": [
    "/images/projects/biocard_digital_biodata/banner.webp"
  ],
  "summary": "An offline-first Android application designed to build, manage, and share comprehensive digital biodata cards with zero external telemetry.",
  "projectDescription": "BioCard transforms physical paper biodata into an elegant, interactive digital profile card on Android. Built with native Java, Android Jetpack, MVVM, and Room SQLite, it provides immediate input validation, complete offline persistence, and seamless system sharing with zero telemetry.",
  "architectureSummary": "Native Android MVVM architecture with Room SQLite persistence, LiveData reactive state, and sandboxed private photo storage.",
  "techStack": [
    "Java",
    "Android SDK",
    "Android Jetpack",
    "Room",
    "SQLite",
    "Material Design",
    "ViewBinding",
    "LiveData",
    "ViewModel",
    "Gradle",
    "JUnit"
  ],
  "telemetryMatrix": {
    "projectType": "Native Android Application",
    "targetPlatform": "Android 8.0+ (API Level 26–36)",
    "primaryDomain": "Digital Identity & Utility",
    "architecturePipeline": "MVVM Clean Architecture & Room",
    "testingAndAudit": "Verified",
    "projectStatus": "Completed",
    "projectYear": "2022"
  },
  "desktopMobileProjectInfo": {
    "applicationType": "Native Android Application",
    "targetPlatform": "Android 8.0 (Oreo) and above",
    "developmentStatus": "Completed",
    "developmentYear": "2022",
    "applicationCategory": "Digital Identity & Portfolio Card"
  },
  "desktopMobileBackground": "Traditional personal and professional biodata forms often rely on fragmented physical paperwork or cumbersome document formats that are difficult to update, verify, and share swiftly. BioCard was engineered to solve this friction by offering a responsive, offline-first digital card with robust local storage and high privacy safeguards.",
  "desktopMobileProblemStatements": [
    {
      "title": "Fragmented Identity Information",
      "description": "Personal and professional data is frequently scattered across disparate formats and hardcopy documents, causing frequent friction during registration and networking.",
      "issueCode": "ISSUE_01"
    },
    {
      "title": "Data Privacy and Telemetry Risks",
      "description": "Cloud-reliant identity management applications introduce data exposure risks and unwanted third-party tracking for sensitive medical and personal details.",
      "issueCode": "ISSUE_02"
    },
    {
      "title": "Complex Form Handling Without Instant Validation",
      "description": "Conventional paper or static forms lack immediate field validation, leading to incomplete submissions, invalid contact formats, and data discrepancies.",
      "issueCode": "ISSUE_03"
    }
  ],
  "desktopMobileObjectives": [
    {
      "title": "Unified Interactive Profile Card",
      "description": "Provide an intuitive single-screen digital card consolidating identity, ICE emergency contacts, education, career, and skills.",
      "targetTag": "TARGET_01"
    },
    {
      "title": "Zero-Permission Privacy & Offline Persistence",
      "description": "Guarantee complete data confidentiality by executing all database transactions locally via Room SQLite without external cloud dependencies.",
      "targetTag": "TARGET_02"
    },
    {
      "title": "Real-Time Validation & Native System Sharing",
      "description": "Implement dynamic client-side field validation and native Android share intent dispatching for instant multi-app interoperability.",
      "targetTag": "TARGET_03"
    }
  ],
  "desktopMobileFeatures": [
    {
      "title": "Multi-Section Biodata Builder",
      "description": "Structured data entry system supporting personal records, emergency contacts, education credentials, career history, and portfolio links.",
      "badge": "Core Profile",
      "metric": "7 Data Categories"
    },
    {
      "title": "System Photo Picker & Avatar Management",
      "description": "Integrates modern Android photo picker to import avatars into private sandbox storage with automatic orphan image garbage collection.",
      "badge": "Privacy Asset",
      "metric": "Zero Permission"
    },
    {
      "title": "Interactive Digital BioCard View",
      "description": "Dynamic card layout with actionable intent links for phone calls, email messaging, external web links, and styled skill chips.",
      "badge": "Visual Card",
      "metric": "One-Tap Action"
    },
    {
      "title": "Universal System Share Sheet",
      "description": "Formats and exports complete biodata records into structured markdown-compatible plain text for distribution across any messaging application.",
      "badge": "Share Utility",
      "metric": "Instant Export"
    }
  ],
  "desktopMobileInterfaceShowcase": [
    {
      "imageUrl": "/images/projects/biocard_digital_biodata/image01.webp",
      "caption": "Interactive splash screen, quick-action home dashboard, and application information interface detailing privacy features.",
      "badge": "Dashboard & Splash"
    },
    {
      "imageUrl": "/images/projects/biocard_digital_biodata/image02.webp",
      "caption": "Full-view digital BioCard showcasing verified contact links, emergency medical data, career credentials, and dynamic skill chips.",
      "badge": "Digital Card View"
    },
    {
      "imageUrl": "/images/projects/biocard_digital_biodata/image03.webp",
      "caption": "Multi-section biodata form highlighting avatar selection, integrated Material date picker, and inline input validation alerts.",
      "badge": "Form & Validation"
    }
  ],
  "desktopMobileUserFlow": {
    "summary": "Users launch the app to access the central dashboard, populate personal and career data through a validated multi-section form with a native date picker, and instantly generate an interactive BioCard that can be previewed, updated, or dispatched directly to external messaging applications via native Android share intents.",
    "steps": [
      {
        "step": "01",
        "title": "Application Launch & Dashboard Access",
        "description": "User opens BioCard; ViewModel observes Room database state and renders either an empty state prompt or active profile card preview.",
        "actorOrNode": "User / MainActivity"
      },
      {
        "step": "02",
        "title": "Data Input & Avatar Selection",
        "description": "User enters profile details, picks birth date via Material DatePicker, and chooses a profile photo using the privacy-safe Android photo picker.",
        "actorOrNode": "User / BiodataActivity"
      },
      {
        "step": "03",
        "title": "Validation & Local Persistence",
        "description": "Input validation rules verify syntax; on confirmation, repository dispatches background worker to commit records to Room SQLite and save avatar.",
        "actorOrNode": "UI Thread / Background Worker"
      },
      {
        "step": "04",
        "title": "Digital Card Presentation & Sharing",
        "description": "User inspects formatted BioCard with interactive action chips, and triggers system share intent to export formatted text to external apps.",
        "actorOrNode": "BioCardActivity / ShareSheet"
      }
    ]
  },
  "desktopMobileArchitecture": {
    "summary": "Engineered using the MVVM architectural pattern, BioCard decouples UI view binding activities from business and data operations. LiveData streams state changes from a local Room database through a repository pipeline, while asynchronous background threads guarantee that all disk and database transactions never block the Android UI thread.",
    "layers": [
      {
        "name": "UI Presentation Layer",
        "role": "Handles user interactions, view inflation via ViewBinding, and reactive lifecycle observation",
        "tech": "Material Design 3 & ViewBinding",
        "components": [
          "MainActivity",
          "BiodataActivity",
          "BioCardActivity",
          "AboutActivity"
        ]
      },
      {
        "name": "ViewModel & Reactive State Layer",
        "role": "Preserves state across configuration changes and exposes observable data streams to UI controllers",
        "tech": "Jetpack ViewModel & LiveData",
        "components": [
          "BiodataViewModel",
          "LiveData Stream"
        ]
      },
      {
        "name": "Repository & Background Execution Layer",
        "role": "Coordinates local persistence, handles photo file sandboxing, and manages asynchronous executor tasks",
        "tech": "Repository Pattern & ExecutorService",
        "components": [
          "BiodataRepository",
          "IO_EXECUTOR ThreadPool",
          "ImageUtils"
        ]
      },
      {
        "name": "Local Persistence & Database Layer",
        "role": "Provides structured relational schema storage with compile-time SQL verification and file storage",
        "tech": "Jetpack Room & SQLite",
        "components": [
          "AppDatabase",
          "BiodataDao",
          "Biodata Entity",
          "Internal Sandbox Files"
        ]
      }
    ]
  },
  "desktopMobileDataManagement": {
    "storageType": "Embedded Relational SQLite",
    "stateEngine": "Jetpack ViewModel & LiveData Observer",
    "offlineSyncStrategy": "100% Local-First Offline Operation",
    "cachingMechanism": "Private App File Sandbox for Profile Media"
  },
  "desktopMobilePlatformImplementation": [
    {
      "title": "Zero-Permission Photo Picker Integration",
      "description": "Leverages Android ActivityResultContracts.PickVisualMedia to access user-selected photos without requiring legacy READ_EXTERNAL_STORAGE runtime permissions.",
      "badge": "Media Sandbox"
    },
    {
      "title": "Sandboxed Profile Photo Garbage Collection",
      "description": "Stores avatar images strictly within internal app files directory (getFilesDir) and systematically deletes unreferenced legacy photos upon update or deletion.",
      "badge": "Storage Cleanup"
    },
    {
      "title": "Native Android Share Intent Pipeline",
      "description": "Assembles formatted multi-section plain text biodata and invokes Android Intent.ACTION_SEND with custom chooser dialogs for universal app sharing.",
      "badge": "System Intents"
    },
    {
      "title": "Strict Background Thread Isolation",
      "description": "Enforces that all database upserts and disk I/O operations execute on an isolated fixed-thread executor, dispatching callbacks back to the main UI thread via Looper.",
      "badge": "Concurrency"
    }
  ],
  "desktopMobileTechSpecs": {
    "programmingLanguage": "Java",
    "framework": "Android SDK",
    "localStorage": "Room SQLite"
  },
  "desktopMobilePlatformSpecs": {
    "targetPlatform": "Android Eight And Above",
    "packageFormat": "Android Package File APK",
    "targetArchitecture": "ARM64 And x86 Architecture",
    "buildFootprint": "Under Ten Megabytes"
  }
}
```
