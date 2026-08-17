---
certifications:
- ISO 27001
- SOC 2
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Donna Trust Center
name_suffix: Trust Center
overview: Donna maintains a public trust center documenting ISO 27001, SOC 2, GDPR, and CCPA compliance.
provider_name: Donna
provider_slug: donna
slug: donna-trust-center
source_filename: donna-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://askdonna.com/enterprise-grade-security\nurl: https://trust.askdonna.com\ncompany: \"Dealside (product: Donna)\"\ncertifications:\n- ISO 27001\n- SOC 2\n- GDPR\n- CCPA\ncontrols:\n- Data encrypted in transit\n- Customer data never used to train AI models\nevidence:\n- source: https://askdonna.com/enterprise-grade-security\n  quote: \"Donna is ISO 27001-certified and fully compliant with GDPR, CCPA, and SOC 2.\"\n- source: https://trust.askdonna.com\n  kind: trust-center\n  note: Live trust portal (JS-rendered) titled \"Dealside Trust Center\"; certification detail\n    behind the portal UI.\nnotes: >-\n  Certification claims captured verbatim from the provider's public security page. No responsible\n  disclosure / bug bounty program is published, and no /.well-known/security.txt was served\n  (HTTP 404), so no VulnerabilityDisclosure artifact is emitted.\nx-recheck:\n  date: '2026-08-14'\n  finding: >-\n    The cited\
  \ source page https://www.askdonna.com/enterprise-grade-security now returns HTTP 301 to\n    the site homepage — it was retired in the 2026-08-03 site rebuild, and the provider's own\n    llms.txt still advertises the dead URL. The certification claims themselves are UNCHANGED and\n    still first-party: the same ISO 27001 / SOC 2 / GDPR / CCPA text is restated verbatim in the\n    current llms.txt (llms/donna-llms.txt), and trust.askdonna.com remains live. The apis.yml\n    Compliance pointer was repointed from the retired page to the live trust center.\n  evidence:\n  - {url: https://www.askdonna.com/enterprise-grade-security, status: 301, location: https://www.askdonna.com/}\n  - {url: https://trust.askdonna.com/, status: 200}\n  - {url: https://www.askdonna.com/llms.txt, status: 200}\n  trust_center_machine_readable: false\n  trust_center_note: >-\n    trust.askdonna.com is a Vanta-hosted single-page app that answers 200 with the same 4.6KB HTML\n    shell for EVERY path (including\
  \ /robots.txt and /sitemap.xml). Certification detail exists only\n    after script execution; api.vanta.com public trust-report endpoints return 401. Nothing\n    machine-readable can be harvested from it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donna/refs/heads/main/security/donna-trust-center.yml
summary_line: ISO 27001, SOC 2, GDPR, CCPA
tags:
- Company
- Artificial Intelligence
- Sales
- Field Sales
- CRM
- Sales Enablement
- Voice AI
- Productivity
- SaaS
- AI Assistant
trust_url: https://trust.askdonna.com
---
