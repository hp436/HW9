# Reflection Document: Key Experiences and Challenges

## Key Experiences

### 1. Database Design and SQL Implementation
I designed relational tables for `users` and `calculations` with appropriate constraints and foreign key dependencies.  
Executing **INSERT**, **SELECT**, **UPDATE**, and **DELETE** queries enhanced my understanding of relational data handling and integrity.  
Performing SQL joins to link user information with calculation records improved my ability to craft efficient queries and navigate data relationships.

### 2. CI/CD Workflow and Automation
Configuring **GitHub Actions** was one of the most impactful parts of this project.  
I developed a pipeline that:
- Executes automated tests with `pytest`
- Runs vulnerability scans using **Trivy**
- Builds and pushes Docker images to **Docker Hub**
- Utilizes `buildx` for cross-platform image creation

This experience gave me practical insight into **continuous integration and continuous deployment**, aligning closely with real-world DevOps processes.

---

## Challenges Faced

### 1. Docker Hub Authentication Issues
One major obstacle was handling **authentication failures** when pushing images to Docker Hub.  
Although credentials were correct, the workflow initially failed due to an **incorrect access token configuration**.  
Through this, I learned to:
- Create a **Personal Access Token (PAT)** in Docker Hub  
- Properly configure **GitHub Secrets** (`DOCKERHUB_USERNAME`, `DOCKERHUB_TOKEN`)
- Confirm authentication locally via `docker login`

This troubleshooting process strengthened my problem-solving skills in managing secure credentials within automated workflows.

### 2. Database Setup in CI Environment
Another challenge involved setting up PostgreSQL as a service in GitHub Actions.  
Ensuring consistent initialization and alignment with local development required careful tuning of **environment variables** and **health checks**.  
Through multiple iterations and tests, I achieved a reliable setup that allowed seamless automated testing.

---

## Reflection
This project provided an end-to-end learning experience combining **data management, containerization, and DevOps automation**.  
I learned to resolve issues methodically—by analyzing logs, adjusting configurations, and validating outcomes iteratively until success.  

In addition to technical growth, I also improved in:
- **Documentation and structured reporting**
- **Version control discipline**
- **Automation-oriented problem-solving**

Overall, the project gave me a holistic understanding of how databases, Docker containers, and CI/CD pipelines integrate to deliver scalable, maintainable, and production-ready systems.

---

## Technologies Utilized
- **PostgreSQL**
- **Docker & Docker Hub**
- **GitHub Actions**
- **Python (pytest)**
- **Trivy Security Scanner**

---
