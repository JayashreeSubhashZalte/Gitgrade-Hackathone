# System Architecture – Stepwise Explanation

## 1. User Submits a Public GitHub Repository URL

**What happens:** The user provides a public GitHub repository link as input to the system.

**Example:**

```
https://github.com/username/project-name
```

**Why this matters:** The repository represents the developer’s real-world work, ensuring evaluation is based on practical output rather than theory.

---

## 2. GitHub API Fetches Repository Metadata

**What happens:** The system uses the GitHub REST API to automatically fetch publicly available repository information.

**Data fetched includes:**

* Folder and file structure
* Programming languages used
* Number of commits
* Commit history and frequency
* Contributors (if any)
* Presence of README.md
* Branch information

**Why this matters:** Provides objective, real data and removes the need for manual inspection.

---

## 3. SonarCloud Performs Static Code Analysis

**What happens:** The repository is connected to SonarCloud, which performs automated static code analysis.

**SonarCloud analyzes:**

* Bugs
* Code smells
* Vulnerabilities
* Code duplication
* Code complexity
* Maintainability rating
* Reliability rating
* Security rating

**Why this matters:** Uses industry-standard tooling to generate quantifiable and reliable code quality metrics.

---

## 4. Analyzer Processes Quality, Structure, and Commit Data

**What happens:** The Analyzer module combines data from GitHub API and SonarCloud.

**Analysis performed:**

* Project organization and modularity
* Documentation quality
* Commit consistency and practices
* Real-world relevance
* Identification of strengths and weaknesses

**Why this matters:** Converts raw metrics into meaningful insights that are easy to understand.

---

## 5. Scoring Engine Calculates Final Score

**What happens:** A weighted scoring system calculates a final score out of 100.

**Scoring parameters:**

* Code Quality
* Project Structure
* Documentation
* Test Coverage
* Real-World Applicability
* Commit Consistency

**Example output:**

```
Final Score: 78 / 100 (Intermediate)
```

**Why this matters:** Provides a clear benchmark to assess repository maturity.

---

## 6. AI Feedback Generator Produces Summary and Roadmap

**What happens:** An AI-driven logic module generates a concise summary and a personalized improvement roadmap.

**Summary example:**

> The repository shows clean structure and good maintainability, but lacks proper documentation and automated tests.

**Roadmap example:**

* Improve README documentation
* Refactor complex methods
* Add unit tests
* Follow Git best practices
* Introduce CI/CD pipelines

**Why this matters:** Acts like an AI coding mentor with actionable guidance.

---

## 7. Final Output Is Displayed to the User

**What happens:** The system presents three final outputs to the user.

**Final outputs:**

1. Score / Rating
2. Written Summary
3. Personalized Roadmap

**Output format:**

```
Score: 78 / 100
Summary: Clean code structure but documentation needs improvement.
Roadmap:
- Improve README
- Add unit tests
- Refactor complex code
```

**Why this matters:** Delivers clear, honest feedback aligned exactly with the hackathon requirements.
