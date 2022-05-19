# DSC HSE, GitHub Actions workshop
 Nizhniy Novgorod, May 2022

# Acronyms

- DevOps - Development and IT Operations
- CI/CD - Continuous Integration / Continuous Delivery (Deployment)
- IaC - Infrastructure as Code

# Schemes

## Extremely simplified architecture of CI based on GitHub Actions

**Pool of jobs (workflow)** → GitHub Actions engine → Pool of runners

## Typical CMake flow

Configure → Build → Test → Install (Pack)

Example
```bash
cmake ..  # Configure
make      # Build
ctest     # Test
cpack     # Pack
```

# Project idea

C++ application that calculates sum of integers starting from 1 to user specified N.
During the workshop serial version of the application will be reworked to parallel to show how dependencies are handled.

The workshop is focused of CI/CD demo, it covers automated build, test (on various Linux distributives) and GitHub release publication.
