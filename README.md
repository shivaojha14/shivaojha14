<!-- ========================================================= -->
<!--                 SHIVAKANT OJHA | GITHUB                   -->
<!--              FULL STACK ENGINEER PORTFOLIO                -->
<!-- ========================================================= --><!-- ================= HERO SECTION ================= --><div align="center"><img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:161B22,100:1F6FEB&height=220&section=header&text=SHIVAKANT%20OJHA&fontSize=48&fontColor=FFFFFF&fontAlignY=38&desc=FULL%20STACK%20ENGINEER%20%7C%20PRODUCT%20BUILDER&descSize=15&descAlignY=58&animation=fadeIn" width="100%" />
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=19&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=700&lines=Engineering+Production-Ready+Applications;Building+Scalable+Backend+Systems;Designing+Reliable+Software+Architecture;Optimizing+Performance+%26+Search;Turning+Business+Problems+Into+Solutions" />


<a href="https://async-shiva-porfolio.vercel.app/">
<img src="https://img.shields.io/badge/PORTFOLIO-Visit%20Website-161B22?style=for-the-badge&logo=vercel&logoColor=white" />
</a>
<a href="https://www.linkedin.com/in/shiva-ojha-356442246/">
<img src="https://img.shields.io/badge/LINKEDIN-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="mailto:ojhashiva139@gmail.com">
<img src="https://img.shields.io/badge/EMAIL-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
</a>


<img src="https://img.shields.io/badge/EXPERIENCE-2%2B%20Years-238636?style=flat-square" />
<img src="https://img.shields.io/badge/FOCUS-Production%20Engineering-1F6FEB?style=flat-square" />
<img src="https://img.shields.io/badge/INTEREST-AI%20Engineering-8957E5?style=flat-square" />


Building software that solves real problems and scales with purpose.
</div><!-- ================= ENGINEERING IDENTITY ================= -->01. / Engineering Identity
I'm Shivakant Ojha, a Full Stack Engineer from India with 2+ years of hands-on experience building and maintaining production web applications.

I work at the intersection of engineering, performance, and business logic.

My experience includes working on live platforms, engineering application workflows, optimizing APIs, implementing search systems, and building solutions designed for real users.

I believe great engineering goes beyond making features work. It's about building systems that are maintainable, reliable, performant, and valuable to the business.
const shiva = {
  role: "Full Stack Engineer",
  experience: "2+ Years",

  engineeringFocus: [
    "Production Web Applications",
    "Scalable Backend Systems",
    "Frontend Architecture",
    "API Development & Optimization",
    "Search & Automation Systems"
  ],

  technologies: {
    frontend: ["React", "Next.js", "TypeScript"],
    backend: ["Node.js", "Express.js"],
    databases: ["MySQL", "MongoDB", "OpenSearch"]
  },

  currentlyExploring: [
    "AI Engineering",
    "LLM Integrations",
    "System Design"
  ],

  philosophy: "Think. Engineer. Optimize. Scale."
};
<!-- ================= SYSTEM ARCHITECTURE ================= -->02. / System Architecture
I approach software development by thinking beyond individual components — focusing on how frontend applications, backend services, APIs, and data systems communicate to deliver reliable products.
01 — Production Web Application Architecture
```mermaid
flowchart TB

    USER(["Users / Admins"])

    subgraph FRONTEND["01. FRONTEND LAYER"]
        direction TB
        UI["Next.js / React.js"]
        STATE["State Management"]
        COMPONENTS["Reusable UI Components"]

        UI --> STATE
        UI --> COMPONENTS
    end

    subgraph BACKEND["02. BACKEND LAYER"]
        direction TB
        API["REST API Layer"]
        AUTH["Authentication & Authorization"]
        LOGIC["Business Logic"]
        VALIDATION["Request Validation"]

        API --> AUTH
        AUTH --> VALIDATION
        VALIDATION --> LOGIC
    end

    subgraph DATA["03. DATA & SEARCH LAYER"]
        direction LR
        DB[("MySQL / MongoDB")]
        SEARCH[("OpenSearch")]
    end

    USER --> UI
    STATE --> API
    LOGIC --> DB
    LOGIC --> SEARCH

    classDef frontend fill:#123B64,stroke:#58A6FF,color:#FFFFFF
    classDef backend fill:#173D32,stroke:#3FB950,color:#FFFFFF
    classDef data fill:#382B55,stroke:#BC8CFF,color:#FFFFFF
    classDef user fill:#1F6FEB,stroke:#79C0FF,color:#FFFFFF

    class UI,STATE,COMPONENTS frontend
    class API,AUTH,LOGIC,VALIDATION backend
    class DB,SEARCH data
    class USER user

```
Architecture principles
- Separation of concerns and modular design.
- Reusable and maintainable frontend components.
- Secure API communication and authentication.
- Structured database management.
- Search integration and efficient data retrieval.
- Performance-oriented application design.
Note: This is a representative architecture of full-stack systems, not a claim that every component is deployed in every project.
02 — Hybrid Search Architecture
One of my interesting engineering areas is working with search functionality, including OpenSearch and keyword-based search.

The following diagram illustrates a conceptual hybrid search workflow.
```mermaid
flowchart TB

    USER(["User Search Query"])

    subgraph PROCESSING["01. QUERY PROCESSING"]
        API["Search API"]
        NORMALIZE["Query Processing & Normalization"]
    end

    subgraph SEARCH["02. SEARCH ENGINES"]
        direction LR
        KEYWORD["Keyword Search"]
        OPENSEARCH["OpenSearch"]
    end

    subgraph AGGREGATION["03. RESULT PROCESSING"]
        MERGE["Result Aggregation"]
        RANK["Filtering & Ranking"]
        RESPONSE["Structured API Response"]
    end

    UI["Frontend Search Results"]

    USER --> API
    API --> NORMALIZE

    NORMALIZE --> KEYWORD
    NORMALIZE --> OPENSEARCH

    KEYWORD --> MERGE
    OPENSEARCH --> MERGE

    MERGE --> RANK
    RANK --> RESPONSE
    RESPONSE --> UI

    classDef input fill:#123B64,stroke:#58A6FF,color:#FFFFFF
    classDef search fill:#382B55,stroke:#BC8CFF,color:#FFFFFF
    classDef process fill:#173D32,stroke:#3FB950,color:#FFFFFF
    classDef output fill:#5A3218,stroke:#D29922,color:#FFFFFF

    class USER,API,UI input
    class KEYWORD,OPENSEARCH search
    class NORMALIZE,MERGE,RANK process
    class RESPONSE output

```
Search engineering concepts
- Query processing and normalization.
- Keyword-based matching.
- OpenSearch integration.
- Result aggregation.
- Relevance-based filtering and ranking.
- Efficient API response handling.
The exact search pipeline depends on the project implementation. This diagram illustrates the general hybrid-search concept.
03 — Software Engineering & CI/CD Lifecycle
Understanding how software moves from development to production is an important part of engineering reliable applications.
```mermaid
flowchart LR

    A["Development"]
    B["Git Commit"]
    C["Pull Request"]
    D["Code Review"]
    E["Automated Testing"]
    F["Build"]
    G["Deployment"]
    H["Production"]
    I["Monitoring"]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
    G --> H
    H --> I

    I -.-> A

    classDef development fill:#123B64,stroke:#58A6FF,color:#FFFFFF
    classDef pipeline fill:#173D32,stroke:#3FB950,color:#FFFFFF
    classDef production fill:#382B55,stroke:#BC8CFF,color:#FFFFFF

    class A,B,C,D development
    class E,F,G pipeline
    class H,I production
```
Engineering workflow principles
- Version control and collaborative development.
- Code reviews and maintainability.
- Automated quality checks and testing.
- Build and deployment processes.
- Production validation and monitoring.
- Continuous improvement.
This represents a reference CI/CD workflow, not a claim that all stages are currently automated in my projects.
<!-- ================= PRODUCTION PROJECTS ================= -->03. / Production Engineering
01 — WholesaleDeals
<a href="https://wholesaledeals.co.uk/">
<img src="https://img.shields.io/badge/LIVE%20PLATFORM-WholesaleDeals-238636?style=flat-square&logo=googlechrome&logoColor=white" />
</a>B2B Wholesale Marketplace

Contributed to a production marketplace connecting suppliers and buyers through deal management and business workflows.

Engineering contributions
- Engineered and optimized deal management functionality.
- Implemented hybrid search using OpenSearch and keyword-based search.
- Worked on API performance optimization and data handling.
- Contributed to supplier and buyer workflow systems.
- Engineered admin panel functionality and management features.
Technology Stack

React.js Next.js Node.js Express.js OpenSearch MySQL
02 — NexBrass
<a href="https://nexbrass.com">
<img src="https://img.shields.io/badge/LIVE%20WEBSITE-NexBrass-238636?style=flat-square&logo=googlechrome&logoColor=white" />
</a>Industrial & Product-Based Business Website

Worked on frontend implementation and website development for an industrial business platform.

Engineering contributions
- Website development and frontend integrations.
- Responsive layouts and user experience improvements.
- Performance and SEO enhancements.
- Reusable interface elements.
Technology Stack

React.js JavaScript HTML CSS SEO
03 — WholesaleLinks India
<a href="https://wholesalelinks.in">
<img src="https://img.shields.io/badge/LIVE%20PLATFORM-WholesaleLinks-238636?style=flat-square&logo=googlechrome&logoColor=white" />
</a>Supplier & Wholesale Directory Platform

Contributed to a directory-style platform designed to organize supplier information and wholesale opportunities.

Engineering contributions
- Frontend system development.
- Data handling and structured content management.
- Feature enhancements and UI improvements.
- Application optimization and maintenance.
Technology Stack

React.js JavaScript REST APIs MySQL
<!-- ================= TECHNICAL SKILLS ================= -->04. / Technical Arsenal
<div align="center">FRONTEND ENGINEERING
<img src="https://skillicons.dev/icons?i=react,nextjs,typescript,javascript,redux,tailwind,html,css" />


BACKEND ENGINEERING
<img src="https://skillicons.dev/icons?i=nodejs,express,java,spring" />


DATABASE & SEARCH
<img src="https://skillicons.dev/icons?i=mongodb,mysql,elasticsearch" />


TOOLS & INFRASTRUCTURE
<img src="https://skillicons.dev/icons?i=git,github,gitlab,docker,linux,postman,vscode" /></div><!-- ================= ENGINEERING FOCUS ================= -->05. / Engineering Focus
Domain	Engineering Focus
Frontend	Component Architecture, State Management, SSR
Backend	REST APIs, Business Logic, Authentication
Database	Query Optimization, Data Modeling
Search	OpenSearch, Keyword Search, Hybrid Search
Performance	API Optimization, SEO, Core Web Vitals
Systems	Automation, Scalable Architecture


<!-- ================= CURRENTLY EXPLORING ================= -->06. / Currently Exploring
01  AI Engineering & LLM-Powered Applications
02  Advanced Next.js Architecture
03  System Design & Distributed Systems
04  Backend Scalability & Performance
05  AI-Powered Business Automation
I'm interested in building intelligent applications that combine modern web technologies with practical AI capabilities.
<!-- ================= GITHUB ANALYTICS ================= -->07. / GitHub Intelligence
<div align="center"><img width="49%" src="https://github-readme-stats.vercel.app/api?username=shivaojha14&show_icons=true&theme=github_dark&hide_border=true&rank_icon=github&include_all_commits=true" /><img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=shivaojha14&layout=compact&theme=github_dark&hide_border=true&langs_count=8" />


<img width="80%" src="https://streak-stats.demolab.com?user=shivaojha14&theme=github-dark-blue&hide_border=true" /></div><!-- ================= BEYOND CODE ================= -->08. / Beyond the Code
- I enjoy understanding complex business requirements.
- I believe clean architecture saves more time than quick fixes.
- I prefer solving real engineering problems over building repetitive demos.
- I continuously explore modern technologies and better engineering practices.
- I believe good software is a combination of technical quality and business value.
<!-- ================= OPPORTUNITIES ================= -->09. / Open to Opportunities
I'm interested in connecting with engineering teams, founders, and companies building meaningful products.

Interested Roles
- Full Stack Engineer
- React.js / Next.js Developer
- Software Engineer
- Full Stack + AI Engineer
Let's build something that matters.
<div align="center"><a href="mailto:ojhashiva139@gmail.com">
<img src="https://img.shields.io/badge/LET'S%20BUILD%20TOGETHER-Contact%20Me-238636?style=for-the-badge&logo=gmail&logoColor=white" />
</a>


<a href="https://github.com/shivaojha14">
<img src="https://img.shields.io/badge/GitHub-shivaojha14-161B22?style=flat-square&logo=github" />
</a><a href="https://www.linkedin.com/in/shiva-ojha-356442246/">
<img src="https://img.shields.io/badge/LinkedIn-Shiva%20Ojha-0A66C2?style=flat-square&logo=linkedin" />
</a>


Think Deeply. Engineer Intelligently. Build Fearlessly.
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1F6FEB,50:161B22,100:0D1117&height=120&section=footer" width="100%" /></div><!-- ========================================================= -->
<!--                  END OF README                            -->
<!-- ========================================================= -->
