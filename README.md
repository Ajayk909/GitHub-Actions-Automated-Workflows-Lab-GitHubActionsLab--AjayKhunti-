# GitHub-Actions-Automated-Workflows-Lab-GitHubActionsLab--AjayKhunti-
# GitHub Actions Automated Workflows Lab

## Workflow 1 – Dependent Jobs

This workflow demonstrates job dependency using GitHub Actions.

Trigger:
It runs automatically when code is pushed to the main branch.

Jobs Included:
1. Build – Simulates building the application.
2. Test – Runs after build using the `needs` keyword.
3. Deploy – Runs after test is completed.

Key Concept:
The `needs` keyword ensures jobs execute in sequence:
Build → Test → Deploy.

---

## Workflow 2 – Multi-Platform Testing

This workflow demonstrates running jobs on multiple operating systems.

Trigger:
It runs when a Pull Request is created to the main branch.

Platforms Tested:
• Ubuntu  
• Windows  
• macOS  

Each job:
- Checks out repository code.
- Displays OS information.
- Creates a file and prints a message like:
  “Hello from Ubuntu”.

Key Concept:
The `runs-on` keyword allows testing on different OS environments simultaneously.

---

## Challenges Faced

- Understanding GitHub Actions folder structure.
- Fixing YAML syntax and trigger errors.
- Learning how Pull Requests trigger workflows.

---

## Conclusion

This lab helped me understand how GitHub Actions automates build, test, and deployment processes and how workflows can run sequentially or in parallel across multiple platforms.
