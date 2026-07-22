---
certifications:
- SOC 2 Type II
- ISO 27001
- B Corporation
description: UpSlide's security & compliance posture, captured from the public "UpSlide Security & Compliance" page (upslide.com/upslide-security/, retrieved 2026-07-21) and the help center's "Architecture and security" section. UpSlide is SOC 2 Type II certified (full report shared with clients on request) and ISO 27001 certified, backed by independent audits. The desktop add-in processes documents locally ("read-only add-in" — no documents, models or deal content stored on UpSlide servers); cloud endpoints run in UpSlide's Microsoft Azure tenant, with AI features on dedicated per-client Azure AI Foundry instances (zero data retention, no training on client data, per-feature model benchmarks). Communications use HTTPS/TLS 1.2 with AES-256 encryption. UpSlide is also a certified B Corporation (linked from upslide.com).
kind: trust-center
layout: security
name: Upslide Trust Center
name_suffix: Trust Center
overview: UpSlide maintains a public trust center documenting SOC 2 Type II, ISO 27001, and B Corporation compliance.
provider_name: UpSlide
provider_slug: upslide
slug: upslide-trust-center
source_filename: upslide-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: false\nurl: https://upslide.com/upslide-security/\ndescription: >-\n  UpSlide's security & compliance posture, captured from the public\n  \"UpSlide Security & Compliance\" page (upslide.com/upslide-security/,\n  retrieved 2026-07-21) and the help center's \"Architecture and security\"\n  section. UpSlide is SOC 2 Type II certified (full report shared with clients\n  on request) and ISO 27001 certified, backed by independent audits. The\n  desktop add-in processes documents locally (\"read-only add-in\" — no\n  documents, models or deal content stored on UpSlide servers); cloud\n  endpoints run in UpSlide's Microsoft Azure tenant, with AI features on\n  dedicated per-client Azure AI Foundry instances (zero data retention, no\n  training on client data, per-feature model benchmarks). Communications use\n  HTTPS/TLS 1.2 with AES-256 encryption. UpSlide is also a certified\n  B Corporation (linked from upslide.com).\ncertifications:\n\
  \  - name: SOC 2 Type II\n    availability: full report shared with clients on request\n    note: >-\n      \"SOC 2 Type II certified ... independently audited and operating\n      effectively over time\" (upslide.com/upslide-security/). Older support\n      article \"Security of UpSlide endpoints\" also states \"UpSlide is SOC-2\n      compliant\" (report via support@upslide.net).\n  - name: ISO 27001\n    note: >-\n      \"UpSlide is fully certified\" against ISO 27001\n      (upslide.com/upslide-security/, retrieved 2026-07-21). Note: the help\n      center article \"AI Security & Data Privacy\" (updated 2026-05-27) still\n      says \"ISO 27001 certification coming soon\"; the newer public security\n      page states full certification.\n  - name: B Corporation\n    note: Certified B Corp (bcorporation.net listing \"pyramid\", linked from upslide.com footer).\nsecurity_practices:\n  - Secure code reviews and code scanning before each release (SANS-based vulnerability rating)\n  - Least-privilege\
  \ access on Azure resources; secrets in Azure Key Vaults; delete locks\n  - Azure Monitor / App Insights monitoring of endpoints\n  - Dedicated per-client Azure AI Foundry; zero retention; prompts/completions not used for training\n  - Auto-update over TLS 1.2 with AES-256 (autoupdate.upslide.net)\ndocs:\n  - https://support.upslide.net/hc/en-us/sections/360004492639-Architecture-and-security\n  - https://support.upslide.net/hc/en-us/articles/360015695439-Security-of-UpSlide-endpoints\n  - https://support.upslide.net/hc/en-us/articles/360015693379-Security-of-UpSlide-software\n  - https://support.upslide.net/hc/en-us/articles/26025072207004-AI-Security-Data-Privacy\n  - https://upslide.com/upslide-security/\nevidence:\n  - source: https://upslide.com/upslide-security/\n    keywords: [soc 2 type ii certified, iso 27001, independently audited, dedicated azure ai foundry, tls 1.2, aes-256]\n  - source: https://support.upslide.net/hc/en-us/articles/360015695439-Security-of-UpSlide-endpoints\n\
  \    keywords: [soc-2 compliant, azure, least privilege, key vaults]\n  - source: https://support.upslide.net/hc/en-us/articles/26025072207004-AI-Security-Data-Privacy\n    keywords: [soc 2 certification standards, iso 27001 coming soon, zero data retention]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upslide/refs/heads/main/security/upslide-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, B Corporation
tags:
- Company
- Applicative Saas
- Document Automation
- Financial Services
- Microsoft 365
- PowerPoint
- Excel
- AI Assistants
- MCP
trust_url: https://upslide.com/upslide-security/
---
