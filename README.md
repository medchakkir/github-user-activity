# GitHub CLI

A command-line tool to manage your GitHub repositories without leaving the terminal — create, list, rename, delete, bulk-rename, export, tag, and clone your repos with simple commands.

Sample solution for the [github-user-activity](https://roadmap.sh/projects/github-user-activity) challenge from [roadmap.sh](https://roadmap.sh/).

## Features

- View recent GitHub activity for any user
- Colorized output for better readability
- Comprehensive error handling
- No external HTTP libraries required
- Supports various event types (pushes, issues, stars, etc.)

## Requirements

- Python 3.6 or higher
- colorama (for Windows compatibility)

## Installation

1. Clone this repository:

```bash
git clone https://github.com/<username>/github-user-activity.git
cd github-user-activity
```

2. Create a virtual environment (optional but recommended):

```bash
python -m venv .venv
.venv/bin/activate  # On Windows
source .venv/bin/activate  # On Linux/MacOS
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

Basic usage:

```bash
python github_activity.py <username>
```

Example:

```bash
python github_activity.py kamranahmedse
```

### Example Output

```
✓ Fetched 5 events for kamranahmedse:
- Pushed 3 commits to kamranahmedse/developer-roadmap
- Opened issue "Update 2024 roadmap" in kamranahmedse/notes
- Starred freeCodeCamp/freeCodeCamp
- Created repository kamranahmedse/todo-cli
- Forked axios/axios to kamranahmedse/axios-fork
```

## Error Handling

The tool handles various error cases:

- Invalid usernames
- API rate limits
- Network errors
- Invalid API responses

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is for educational purposes.
