<!-- Improved compatibility of back to top link -->

<a id="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">

  <h3 align="center">KYC Privacy Gateway (KPG)</h3>

  <p align="center">
    Protecting sensitive customer data during AI-assisted KYC checks.
    <br />
    <a href="https://github.com/breadonhtw/KYC-Private-Gateway-KPG-#"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="">View Demo</a>
    ·
    <a href="https://github.com/breadonhtw/KYC-Private-Gateway-KPG-/issues/new">Report Bug</a>
    ·
    <a href="https://github.com/breadonhtw/KYC-Private-Gateway-KPG-/issues/new">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## About The Project

**KYC Privacy Gateway (KPG)** solves a critical challenge for financial institutions:  
How can analysts use AI tools like Microsoft Copilot or LLMs for background checks **without leaking customer PII**?

Traditional AI prompts risk exposing high-value customer names, IDs, and accounts outside the bank’s environment. KPG sits as a **privacy gateway**:

- Detects and tokenises PII (NRIC, Passport, Account numbers, Names).
- Performs **internal searches** using the real identifiers.
- Sends only **sanitised excerpts + subject tokens** to LLMs for summarisation.
- Provides an **auditable log** of every step.

**Hackathon Tracks:**

- Track 7: _Privacy Meets AI_
- Track 4: _Building UI for the AI Era with Lynx_ (optional challenge)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

- [![Lynx][Lynx.js]][Lynx-url]
- [![FastAPI][FastAPI]][FastAPI-url]
- [![Python][Python]][Python-url]
- [![React][React.js]][React-url]
- [![OpenAI][OpenAI]][OpenAI-url]
- [![Presidio][Presidio]][Presidio-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->

## Getting Started

### Prerequisites

You’ll need:

- Python 3.10+
- Node.js & NPM
- OpenAI API key (or Azure OpenAI endpoint)

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/your-username/kpg.git
   cd kpg
   ```
2. Backend Setup (FastAPI)
   ```sh
   cd backend
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   uvicorn main:app --reload
   ```
3. Frontend Setup (Lynx)
   ```sh
   cd ../frontend
   npm install
   npm run dev
   ```
4. Confirm Connectivity
   - Backend API should be running at `http://localhost:8000`
   - Frontend should be accessible at `http://localhost:3000`
5. Optional: Run with Docker
   ```sh
   docker-compose up --build
   ```
   This will start both backend and frontend services in containers.

<!-- Reference-style image definitions -->

[Lynx.js]: https://img.shields.io/badge/Lynx.js-2D2D2D?style=for-the-badge&logo=react&logoColor=white
[Lynx-url]: https://lynxjs.org/
[Lynx-url]: https://lynx.sh/
[FastAPI]: https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white
[FastAPI-url]: https://fastapi.tiangolo.com/
[Python]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
[Python-url]: https://www.python.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://react.dev/
[OpenAI]: https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white
[OpenAI-url]: https://openai.com/
[Presidio]: https://img.shields.io/badge/Presidio-0078D4?style=for-the-badge&logo=microsoft&logoColor=white
[Presidio-url]: https://microsoft.github.io/presidio/
