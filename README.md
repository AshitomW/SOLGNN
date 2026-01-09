# Installation Guide

This guide will help you set up your development environment using UV, a fast Python package installer and resolver.

## Prerequisites

- Python 3.8 or higher installed on your system
- pip (usually comes with Python)

## Step-by-Step Installation

### 1. Install UV

First, install UV using pip:

```bash
pip install uv
```

UV is a modern Python package installer that's significantly faster than traditional pip. It provides better dependency resolution and improved caching.

### 2. Create Virtual Environment

Create a new virtual environment for your project:

```bash
uv venv
```

This creates a `.venv` directory in your project folder containing an isolated Python environment.

### 3. Activate Virtual Environment

Before installing packages, activate your virtual environment:

**On Windows:**

```bash
.venv\Scripts\activate
```

**On macOS/Linux:**

```bash
source .venv/bin/activate
```

### 4. Install Required Packages

Install all project dependencies from the requirements file:

```bash
uv pip install -r requirements.txt
```

## Verification

To verify your installation was successful:

```bash
python --version
pip list
```

## Troubleshooting

- **UV not found**: Make sure pip's installation directory is in your PATH
- **Permission errors**: Try using `pip install --user uv` instead
- **Virtual environment issues**: Delete the `.venv` folder and recreate it

## Next Steps

Your environment is now ready! You can start developing by running your main application script or exploring the project files.

To deactivate the virtual environment when you're done:

```bash
deactivate
```
