## 🍎 Spec-Kit Plus Installation & Setup (macOS)

Spec-Kit Plus is a structured AI development framework that organizes your workflow using **Spec-Driven Development (SDD): Specifications → Plans → Tasks → Code**.

This guide provides a complete, correct, and ready-to-download setup for **macOS** users.

-----

### Prerequisites

Ensure the following before you begin. You can use your Mac's **Terminal** application for these checks.

  * **Python 3.12 or higher**

    ```bash
    python3 --version
    ```

  * **Optional: Git for version control** (Usually pre-installed on macOS)

    ```bash
    git --version
    ```

-----

### Install Spec-Kit Plus CLI

Open **Terminal** and use **`pip`** to install the package.

```bash
pip3 install specifyplus
```

**Verify the installation:**

```bash
specifyplus --version
```

**Check available command options:**

```bash
specifyplus --help
```

-----

### Initialize a New Project

**1. Navigate to your desired folder:**

```bash
cd ~/Desktop/
# or
cd /path/to/your/project
```

**2. Initialize a new Spec-Kit Plus project:**

```bash
specifyplus init my-project-name
```

During setup, you will select:

  * Your AI tool (**Claude Code** or **Gemini CLI**)
  * Terminal type (Default **zsh** or **bash** is recommended)

**3. Move into your new project:**

```bash
cd my-project-name
```

-----

### Verify Project Structure

After initialization, your project should contain this structure:

```
my-project-name/
├── .claude/
│   └── commands/
├── .specify/
│   ├── memory/
│   ├── scripts/
│   └── templates/
├── .git/ (If Git was selected)
├── CLAUDE.md
├── README.md
└── .gitignore
```

As you proceed, directories such as `specs/` and `history/` will appear.

-----

### Test Spec-Kit Plus Commands

**1. Launch your chosen AI tool:**

```bash
claude   # or
gemini
```

**2. Then type the main command:**

```bash
/sp.
```

You should see commands like:

```
/sp.constitution
/sp.specify
/sp.clarify
/sp.plan
/sp.adr
/sp.tasks
/sp.implement
/sp.phr
```

If these appear, **Spec-Kit Plus** is working properly.

-----

### Update Spec-Kit Plus

Keep your installation up to date:

```bash
pip3 install --upgrade specifyplus
```

-----

### Common Pitfalls

  * Installing only the AI tool — **Spec-Kit Plus** must be installed separately.
  * Running Python older than **3.12**.
  * Manually creating project folders instead of using `specifyplus init`.

-----

### Quick Start Commands

```bash
python3 --version
pip3 install specifyplus
specifyplus init my-first-project
cd my-first-project
claude   # or gemini
/sp.
```
thanks
