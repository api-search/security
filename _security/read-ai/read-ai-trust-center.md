---
certifications:
- SOC 2 Type 2
- HIPAA
- GDPR
- EU-U.S. Data Privacy Framework
description: Read AI runs a Vanta-hosted Trust Center at trust.read.ai. The page itself is a client-rendered single-page app — the only text a fetch returns is the title "Read AI Trust Center", and every /api/* path answers 200 with the same HTML shell — so the certification list below is taken from Read AI's own Security & Privacy Overview help article, which names what the Trust Center holds. The documents themselves are behind the Trust Center's request/NDA flow and were not fetched.
kind: trust-center
layout: security
name: Read Ai Trust Center
name_suffix: Trust Center
overview: Read AI maintains a public trust center documenting SOC 2 Type 2, HIPAA, GDPR, and EU-U.S. Data Privacy Framework compliance.
provider_name: Read AI
provider_slug: read-ai
slug: read-ai-trust-center
source_filename: read-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: true\nurl: https://trust.read.ai/\ndescription: >-\n  Read AI runs a Vanta-hosted Trust Center at trust.read.ai. The page itself is a\n  client-rendered single-page app — the only text a fetch returns is the title \"Read\n  AI Trust Center\", and every /api/* path answers 200 with the same HTML shell — so\n  the certification list below is taken from Read AI's own Security & Privacy Overview\n  help article, which names what the Trust Center holds. The documents themselves are\n  behind the Trust Center's request/NDA flow and were not fetched.\nplatform: Vanta\ncertifications:\n  - name: SOC 2 Type 2\n    claimed_at: https://support.read.ai/hc/en-us/articles/25702259763091-Security-Privacy-Overview\n    artifact_access: request via https://trust.read.ai/\n  - name: HIPAA\n    note: Listed as an Enterprise+ plan capability; BAA available.\n    claimed_at: https://www.read.ai/plans-pricing\n  - name: GDPR\n    claimed_at: https://support.read.ai/hc/en-us/articles/25702259763091-Security-Privacy-Overview\n\
  \  - name: EU-U.S. Data Privacy Framework\n    claimed_at: https://support.read.ai/hc/en-us/articles/25702259763091-Security-Privacy-Overview\n    independently_verifiable_at: https://www.dataprivacyframework.gov/list\ndocuments_referenced:\n  - SOC 2 Type 2 report\n  - Data Processing Agreement\n  - Other compliance forms\nrelated_public_pages:\n  - {name: Security & Privacy Overview, url: 'https://support.read.ai/hc/en-us/articles/25702259763091-Security-Privacy-Overview'}\n  - {name: Data Processing Addendum, url: 'https://www.read.ai/data-processing-addendum'}\n  - {name: Privacy Policy, url: 'https://www.read.ai/privacy-policy'}\n  - {name: 'Workspace Audit Logs (OCSF 1.7.0)', url: 'https://support.read.ai/hc/en-us/articles/50196944604563-Workspace-Audit-Logs-Event-Types-and-Schema'}\nsecurity_practices_claimed:\n  - Regular SOC 2 audits and penetration tests\n  - Encryption in transit and at rest\n  - Data stored in AWS us-east-1 (Northern Virginia, USA)\n  - SSO, SAML, SCIM and\
  \ two-factor authentication\n  - User-set data retention policies\n  - Customer data not used to train AI models\nevidence:\n  - {source: 'https://trust.read.ai/', http_status: 200, observed: 'Vanta trust-report SPA; title \"Read AI Trust Center\"'}\n  - {source: 'https://support.read.ai/hc/en-us/articles/25702259763091-Security-Privacy-Overview', http_status: 200, keywords: ['soc 2 type 2', 'trust center', 'data privacy framework', gdpr, hipaa, 'penetration tests']}\nx-evidence:\n  fetched: '2026-08-05'\n  note: >-\n    The automated probe (0-working/probe-security-programs.py) returned trust=none\n    because the SPA body carries fewer than two trust keywords. This file supersedes\n    that null with a docs-searched result.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/read-ai/refs/heads/main/security/read-ai-trust-center.yml
summary_line: SOC 2 Type 2, HIPAA, GDPR, EU-U.S. Data Privacy Framework
tags:
- Company
- Meeting Intelligence
- Artificial Intelligence
- Transcription
- Productivity
- Collaboration
- Model Context Protocol
- Agents
- Webhooks
- SaaS
trust_url: https://trust.read.ai/
---
