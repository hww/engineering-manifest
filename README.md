# Engineering File Naming & Organization Manifest

[![License: MIT](https://shields.io)](https://opensource.org)

A battle-tested standard for organizing engineering projects, CAD libraries, and development environments across **Altium, KiCad, CCES**, and more. It introduces a strict 3-level hierarchy, clean naming conventions, and automated tooling to eliminate chaos in hardware and software design.

📖 **[Читать на русском языке (manifest.ru.md)](manifest.ru.md)**
📖 **[Read English version (manifest.en.md)](manifest.en.md)**

---

## 🚀 Key Features

* **3-Level Hierarchy** — Clear separation from root workspace down to project-specific assets.
* **CAD & IDE Friendly** — Native structure optimization for Altium Designer, KiCad, and CrossCore Embedded Studio.
* **Strict Naming Conventions** — Predictable, machine-readable file and folder names.
* **Automated Tooling** — Scripts to validate and generate compliant project templates.

---

## 📁 Repository Structure

```text
├── LICENSE
├── README.md               # English introduction & quick start
├── manifest.ru.md          # Full manifest specification (Russian)
└── [tools/]*               # (Optional) Automation scripts and templates
```

---

## 🛠️ The 3-Level Hierarchy Concept

Our manifest enforces a strict breakdown to ensure that any engineer can navigate any project instantly:

1. **Level 1: Global Workspace (`/PRJ/`)** — The entry point for all engineering activities.
2. **Level 2: Category / Client (`/PRJ/CLIENT_OR_CATEGORY/`)** — Grouping projects by ownership or domain.
3. **Level 3: Target Project (`/PRJ/CLIENT/PROJECT_NAME/`)** — Isolated development environment containing hardware (CAD), software (IDE), and documentation.

### Quick Example:
```text
/mnt/d/projects/
└── hww/
    └── engineering-manifest/
        ├── hardware/       # Altium / KiCad schematics and PCBs
        ├── firmware/       # CCES / MCU source code
        └── docs/           # Datasheets and production files
```

---

## 📝 Naming Rules Cheat Sheet

* **Case Style:** Use `kebab-case` or `snake_case` (consistently) based on your language environment. Avoid spaces.
* **Date Format:** Always use `YYYY-MM-DD` for changelogs or manual archives.
* **Version Control:** Match Git tags with your hardware/firmware revision numbers (e.g., `v1.0.0`).

---

## ⚙️ Getting Started

1. Read the full **[Manifest Specification](manifest.ru.md)** to understand the rules.
2. Clone this repository to use it as a reference or a base boilerplate.
3. Apply the structure to your new or existing engineering project.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
