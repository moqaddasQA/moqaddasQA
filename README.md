<div align="center">
  <img src="https://i.imgur.com/WThKn1B.png" alt="QA Automation Banner" width="100%" style="border-radius: 10px; margin-bottom: 20px;">

  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com/?lines=Hello,+There!+👋;I+am+Moqaddas+Rahim;Architect+of+Quality+&amp;+Automation.&center=true&size=30&color=F7F7F7&background=00000000&vCenter=true&width=600&height=50" alt="Typing SVG" />
  </a>

  <p style="font-style: italic; font-size: 1.2em; max-width: 600px; margin: 10px auto;">
    "Located at the crossroads of creativity and excellence, I develop automation solutions that transform how products are tested and refined."
  </p>

  <a href="https://www.linkedin.com/in/moqaddas-qa-automation" target="_blank">
    <img src="https://img.shields.io/badge/HIRE%20ME-Connect%20on%20LinkedIn-27ae60?style=for-the-badge&logo=linkedin&logoColor=white" height="40" alt="Hire Me"/>
  </a>
</div>

<br />

## ⚙️ Technical Arsenal

| **Core Frameworks** | **CI/CD & Management** | **Data & Platform** |
|:---:|:---:|:---:|
| <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" height="30"/> <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" height="30"/> <br> <img src="https://img.shields.io/badge/Cucumber-23D18B?style=for-the-badge&logo=cucumber&logoColor=white" height="30"/> <img src="https://img.shields.io/badge/Rest_Assured-025C51?style=for-the-badge&logo=postman&logoColor=white" height="30"/> | <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white" height="30"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" height="30"/> <br> <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" height="30"/> <img src="https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white" height="30"/> | <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" height="30"/> <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" height="30"/> <br> <img src="https://img.shields.io/badge/Appium-41B883?style=for-the-badge&logo=appium&logoColor=white" height="30"/> <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" height="30"/> |

---

## 🏗️ Automation Architecture

```mermaid
graph TD
  %% Theme Configuration
  classDef trigger fill:#f9f,stroke:#333,stroke-width:2px;
  classDef exec fill:#bbf,stroke:#333,stroke-width:2px;
  classDef data fill:#dfd,stroke:#333,stroke-width:2px;

  subgraph CI_CD_Pipeline [CI/CD Pipeline]
    A[Code Commit / GitHub] -->|Trigger| B[Jenkins CI]
    B -->|Build| C{Test Strategy}
  end

  subgraph Execution_Layer [Test Execution]
    C -->|UI Tests| D[Selenium Grid]
    C -->|API Tests| E[REST Assured]
    C -->|Mobile| F[Appium]
  end

  subgraph Reporting_Compliance [Reporting & Data]
    D & E & F --> G[Allure Reports]
    D & E & F --> H[(MySQL / Oracle)]
    G --> I[Jira Dashboard]
    I --> J[Compliance: HIPAA / PCI-DSS]
  end

  class A,B trigger;
  class D,E,F exec;
  class H,J data;
