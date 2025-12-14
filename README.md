# Gitgrade-Hackathone
Gitgrade-Hackathone
# GitGrade – AI-Powered GitHub Repository Evaluation System

## Hackathon Theme
AI + Code Analysis + Developer Profiling

## Problem Statement
Students often struggle to understand how good their GitHub repositories look to recruiters.
GitGrade acts as a Repository Mirror by analyzing a GitHub repository and generating a score,
summary, and personalized improvement roadmap.

## Solution Overview
GitGrade accepts a public GitHub repository URL and evaluates it using GitHub APIs and
SonarCloud. Based on real code metrics, the system provides honest feedback and actionable
guidance.

## System Architecture
User → GitHub Repository URL → GitHub API + SonarCloud → Analyzer Engine → Scoring Engine →
AI Feedback Generator → Score + Summary + Roadmap

## Tools Used
- GitHub REST API
- SonarCloud (Static Code Analysis)
- GitHub Actions
- Python (conceptual backend)

## Evaluation Dimensions
- Code Quality & Readability
- Project Structure & Organization
- Documentation & Clarity
- Test Coverage & Maintainability
- Real-World Applicability
- Commit Consistency

## Output
### Score
Score out of 100 based on weighted evaluation.

### Summary
Short recruiter-style evaluation of the repository.

### Personalized Roadmap
Actionable steps to improve code quality, documentation, testing, and Git practices.

## Sample Input
https://github.com/username/project-name

## Sample Output
Score: 78 / 100  
Summary: Clean structure but documentation and tests need improvement.  
Roadmap:
- Improve README
- Add unit tests
- Refactor complex methods
- Introduce CI/CD

## Conclusion
GitGrade provides accurate analysis, honest feedback, and an actionable roadmap, helping
students improve their GitHub repositories in a recruiter-friendly way.
