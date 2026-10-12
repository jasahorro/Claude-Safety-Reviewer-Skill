<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Do this before downloading any MCP or Skill

**Project Link:** [View Project](https://nextwork.ai/projects/e933f851-f343-4108-adbb-e62482dede58)

**Author:** Maria Jasmin Ahorro  
**Email:** jasminahorro23@gmail.com

---

![Image](https://nextwork.ai/overjoyed_magenta_proud_yak/uploads/e933f851-f343-4108-adbb-e62482dede58_txyoanug)

## Project Overview

### Goals and objectives

In this project, I'm building a personal safety-checking workflow powered by Claude so that I can vet MCP servers, extensions, and skills for security risks before installing them.

## Configuring Claude with Custom Skills

### Setting up the environment

In this step, I'm setting up my Claude environment and enabling code execution so that I can prepare Claude to run custom skills and securely test third-party extensions.

![Image](https://nextwork.ai/overjoyed_magenta_proud_yak/uploads/e933f851-f343-4108-adbb-e62482dede58_1lue1uus)

## Running a Structured Safety Analysis

### Approach and methodology

In this step, I'm learning how to perform a structured six-point safety analysis on external code so that I can reliably vet MCP servers and skills for permissions, dependencies, and hidden risks before installation.

### Naive vs. structured responses

The naive response was a brief, vague, and unpredictable reassurance that merely glanced at the top-level repository description without verifying underlying code paths or security implications while the structured response showed me a rigorous, multi-point security audit covering six critical risk areas—permissions, dependencies, network access, data exposure, author trust, and red flags—backed by a clear trust verdict.

## Deploying a Custom Safety-Reviewer Skill

![Image](https://nextwork.ai/overjoyed_magenta_proud_yak/uploads/e933f851-f343-4108-adbb-e62482dede58_r8ykcx46)

### Confirming automatic skill triggers

In this project extension, I tested my custom safety-reviewer skill by pasting the GitHub repository link for obra/superpowers to evaluate how effectively the automated workflow handles complex third-party tools and plugins. Rather than requiring me to manually paste an exhaustive, multi-line prompt, the custom skill recognized the context instantly upon encountering the repository URL and initiated a rigorous, automated audit in the background.

The response included a comprehensive and well-structured security analysis covering six vital risk areas. First, it inspected Permissions, noting that the plugin primarily consists of instruction markdown files alongside a startup hook that reads its own documentation and formats it as JSON without executing unauthorized file writes or secret reads. Second, it evaluated Dependencies, confirming that the configuration files contain zero external packages, third-party modules, or post-install scripts. Third, it checked Network Access, identifying a single opt-out telemetry call that loads a version-check logo from the developer's website while properly respecting standard telemetry-disable environment variables. Fourth, it reviewed Data Exposure, verifying that the system does not passively capture local credentials, active conversation histories, or sensitive environment variables. Fifth, it assessed Author Trust, highlighting the active maintenance by a recognized open-source developer and the repository's widespread community adoption. Finally, it analyzed Red Flags, noting that while the prompt phrasing is deliberately forceful to enforce test-driven development and strict brainstorming loops, it represents workflow preferences rather than malicious obfuscation or hidden security vectors.

The evaluation concluded with a clear trust verdict of caution accompanied by practical installation instructions, demonstrating that my custom skill successfully automates the entire vetting process and provides a reliable safety baseline.

## Reflections and Key Takeaways

### Tools and concepts learned

The key tools I used include Claude's cloud code execution environment, custom skill packaging and upload features under the Customize and Skills panel, and Anthropic's public GitHub repository containing the skill-creator framework.

Key concepts I learnt include understanding the vulnerabilities of third-party extensions, recognizing the unpredictability of unstructured prompts versus structured queries, executing a rigorous six-point security analysis covering permissions, dependencies, network access, data exposure, author trust, and red flags, and building automated custom skills that trigger automatically upon encountering external repository links.

### Time and challenges

This project took me approximately 20 minutes to complete. The most challenging part was understanding how to structure the custom skill's trigger descriptions effectively so that Claude automatically invokes the six-point safety review when encountering repository links without needing manual prompt injection.

### Looking ahead

I did this project today to learn how to build a repeatable safety-checking workflow and custom Claude skill to vet third-party extensions and MCP servers for security risks. Another skill I want to learn is how to build automated Model Context Protocol (MCP) servers to integrate custom databases and external APIs directly into Claude.

---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/e933f851-f343-4108-adbb-e62482dede58)*
