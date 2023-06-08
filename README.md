    <h1 align="center">BYTE CHAT</h1>
  </a>
</p>

<p align="center">
  <a aria-label="Join the community on Discord" href="https://discord.gg/XwuaaRJQ">
  </a>
</p>

# Features

- Response streaming identical to ChatGPT through server-sent events
- UI from original ChatGPT, including Dark mode
- AI model selection (through 3 endpoints: OpenAI API, BingAI, and ChatGPT Browser)
- Create, Save, & Share custom presets for OpenAI and BingAI endpoints - [More info on customization here](https://github.com/danny-avila/chatgpt-clone/releases/tag/v0.3.0)
- Edit and Resubmit messages just like the official site (with conversation branching)
- Search all messages/conversations - [More info here](https://github.com/danny-avila/chatgpt-clone/releases/tag/v0.1.0)
- Integrating plugins soon


## **Google's PaLM 2 is now supported as of [v0.4.3](https://github.com/danny-avila/chatgpt-clone/releases/tag/v0.4.3)**
  
  ![image](https://github.com/danny-avila/chatgpt-clone/assets/110412045/ec5e8ff3-6c3a-4f25-9687-d8558435d094)
 
<details>
<summary><strong>How to Setup PaLM 2 (via Google Cloud Vertex AI API)</strong></summary>
- Enable the Vertex AI API on Google Cloud:
- - https://console.cloud.google.com/vertex-ai
- Create a Service Account:
- - https://console.cloud.google.com/projectselector/iam-admin/serviceaccounts/create?walkthrough_id=iam--create-service-account#step_index=1
- Make sure to click 'Create and Continue' to give at least the 'Vertex AI User' role.
- Create a JSON key, rename as 'auth.json' and save it in /api/data/.

**Alternatively**

- In your ./api/.env file, set PALM_KEY as "user_provided" to allow the user to provide a Service Account key JSON from the UI.
- They will follow the steps above except for renaming the file, simply importing the JSON when prompted.
- The key is sent to the server but never saved except in your local storage

**Note:**

- Vertex AI does not (yet) support response streaming for text generations, so response may seem to take long when generating a lot of text.
- Text streaming is simulated
</details>

---

## [Read all Latest Updates here](CHANGELOG.md)

<h1>Table of Contents</h1>

<details open>
  <summary><strong>Getting Started</strong></summary>

  * [Docker Install](/documents/install/docker_install.md)
  * [Linux Install](documents/install/linux_install.md)
  * [Mac Install](documents/install/mac_install.md)
  * [Windows Install](documents/install/windows_install.md)
</details>

<details>
  <summary><strong>General Information</strong></summary>

  * [Project Origin](documents/general_info/project_origin.md)
  * [Multilingual Information](documents/general_info/multilingual_information.md)
  * [Roadmap](documents/general_info/roadmap.md)
  * [Tech Stack](documents/general_info/tech_stack.md)
  * [Changelog](CHANGELOG.md)
  * [Bing Jailbreak Info](documents/general_info/bing_jailbreak_info.md)
</details>

<details>
  <summary><strong>Features</strong></summary>

  * [User Auth System](documents/features/user_auth_system.md)
  * [Proxy](documents/features/proxy.md)
</details>

<details>
  <summary><strong>Cloud Deployment</strong></summary>

  * [Heroku](documents/deployment/heroku.md)
</details>

<details>
  <summary><strong>Contributions</strong></summary>

  * [Code of Conduct](documents/contributions/code_of_conduct.md)
  * [Contributor Guidelines](documents/contributions/contributor_guidelines.md)
  * [Documentation Guidelines](documents/contributions/documentation_guidelines.md)
  * [Code Standards and Conventions](documents/contributions/coding_conventions.md)
  * [Testing](documents/contributions/testing.md)
  * [Security](SECURITY.md)
  * [Contributors](CONTRIBUTORS.md)
  * [Trello Board](https://trello.com/b/17z094kq/chatgpt-clone)
</details>
