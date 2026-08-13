---
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Leadpages Trust Center
name_suffix: Trust Center
overview: Leadpages maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: Leadpages
provider_slug: leadpages
slug: leadpages-trust-center
source_filename: leadpages-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nsource: https://leadpages.com/security\nurl: https://leadpages.com/security\nnote: >-\n  Leadpages publishes a security page rather than a dedicated trust center — there is\n  no trust.leadpages.com, no control portal and no downloadable evidence pack. The page\n  does describe practices, infrastructure and a responsible-disclosure program in\n  detail, so it is captured here as the trust surface.\ncertifications:\n- name: SOC 2 Type II\n  status: in-progress\n  claim_verbatim: >-\n    We are actively pursuing SOC 2 Type II certification. Our security controls are\n    designed to meet the Trust Service Criteria for security, availability, and\n    confidentiality.\n  note: >-\n    IMPORTANT — this is a stated intent, NOT a held certification. The automated\n    keyword probe recorded \"SOC 2\" as a certification; that has been corrected here\n    against the page text. No report, auditor or observation period is published.\n\
  - name: GDPR\n  status: claimed-compliant\n  claim_verbatim: >-\n    We support data subject access requests, right to deletion, and data portability.\n    Our infrastructure and data processing practices meet GDPR requirements.\n  supporting_page: https://leadpages.com/legal/gdpr\nnot_claimed:\n- ISO 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\n- CSA STAR\npractices:\n- {area: encryption_in_transit, detail: HTTPS with TLS 1.3 on every page, custom domain and API endpoint; free SSL auto-provisioned for custom domains}\n- {area: encryption_at_rest, detail: AES-256; database backups, file storage and sensitive fields encrypted independently with managed keys}\n- {area: authentication, detail: OAuth 2.0 and bearer tokens for API and MCP integrations; credentials not shared with third-party tools or AI agents}\n- {area: content_safety, detail: every page scanned for malicious content on publish; phishing, malware and abuse flagged before reaching visitors}\n- {area: ddos, detail: all traffic routed\
  \ through Cloudflare global CDN for DDoS mitigation, rate limiting and bot management at the edge}\n- {area: audits, detail: regular internal security reviews and vulnerability assessments; dependencies continuously monitored for known vulnerabilities}\ninfrastructure:\n  cdn: Cloudflare, 330+ edge locations\n  hosting: AWS — ECS Fargate, Aurora Serverless, ElastiCache\n  database: PostgreSQL with encryption at rest, automated daily backups, point-in-time recovery\n  object_storage: Cloudflare R2 (encrypted)\n  uptime_sla: 99.9%\n  edge_response_time: <50ms\ndata_handling:\n  third_party_sharing: >-\n    States data is never sold or shared with third parties for marketing purposes;\n    shared only with infrastructure providers (AWS, Cloudflare) as necessary to operate\n    the service, under contractual protection.\n  data_residency: AWS Aurora (region not published)\ncontacts:\n  security: security@leadpages.com\n  privacy: privacy@leadpages.com\n  support: support@leadpages.com\nevidence:\n\
  - source: https://leadpages.com/security\n  http_status: 200\n  keywords: [soc 2, gdpr, tls 1.3, aes-256, responsible disclosure, uptime sla]\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - {url: 'https://leadpages.com/security', status: 200}\n  - {url: 'https://leadpages.com/legal/gdpr', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadpages/refs/heads/main/security/leadpages-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Company
- Landing Pages
- Marketing
- Conversion Optimization
- A/B Testing
- Website Builder
- Lead Generation
- Content Management
- Agents
- Analytics
trust_url: https://leadpages.com/security
---
