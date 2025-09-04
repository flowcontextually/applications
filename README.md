# Contextually Applications

Welcome to the official public registry for **Contextually Applications**! This repository is the central "App Store" for the `cx` ecosystem, providing discoverable, installable, and community-vetted solutions.

An Application is a self-contained, versioned package that solves a specific business problem. It bundles all the necessary flows, queries, and scripts into a "toolkit-in-a-box" that you can install with a single command.

[**Learn more about the Application Ecosystem in our official documentation.**](https://flowcontextually.github.io/docs/concepts/application-ecosystem/)

---

## 🚀 How to Use Applications

You don't need to clone this repository to use these applications! The `cx` shell (`v0.3.0` and later) handles everything for you.

1.  **Search for an Application:**
    ```bash
    cx app search github
    ```

2.  **Install an Application:**
    ```bash
    cx app install official/github-repo-manager
    ```
    The `cx` shell will download the application, resolve its blueprint dependencies, and guide you through an interactive setup for any required connections.

---

## 📦 Available Applications

This is the official catalog of applications.

### Official Applications (`official/`)

These are core applications maintained directly by the Contextually team.

| Application ID | Latest Version | Description |
| :--- | :--- | :--- |
| [`official/github-repo-manager`](./official/github-repo-manager/) | `v1.0.0` | A suite of flows for managing GitHub repository settings, labels, and collaborators. |

### Community Applications (`community/`)

These are applications contributed and maintained by our open-source community.

*(This table will grow as the community contributes more applications!)*

---

## 🤝 How to Contribute

Contributing a new application is a fantastic way to support the Contextually ecosystem. The process is streamlined for developers.

1.  Build your application's assets (`flows/`, `queries/`, etc.) in a local directory.
2.  Create an `app.cx.yaml` manifest file at the root.
3.  Use the `cx app package` command to create a distributable archive.
4.  Submit a Pull Request to this repository, adding your application's source code to the `community/` directory and adding an entry to the `registry.yaml` file.

For a detailed guide, please see our `CONTRIBUTING.md` file (to be created).
