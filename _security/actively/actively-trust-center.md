---
certifications:
- SOC 2 Type II
- ISO 27001
- HITRUST
- GDPR
- CCPA
description: Actively AI operates a public trust center at trust.actively.ai — a Vanta Trust Center on the company's own subdomain. It is the customer-facing surface for security documentation, complementing the narrative security page at www.actively.ai/security.
kind: trust-center
layout: security
name: Actively Trust Center
name_suffix: Trust Center
overview: Actively maintains a public trust center documenting SOC 2 Type II, ISO 27001, HITRUST, GDPR, and CCPA compliance.
provider_name: Actively
provider_slug: actively
slug: actively-trust-center
source_filename: actively-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://trust.actively.ai/\nname: Actively Trust Center\nurl: https://trust.actively.ai/\ndescription: >-\n  Actively AI operates a public trust center at trust.actively.ai — a Vanta\n  Trust Center on the company's own subdomain. It is the customer-facing\n  surface for security documentation, complementing the narrative security\n  page at www.actively.ai/security.\nplatform:\n  vendor: Vanta\n  evidence: >-\n    The page is served from Actively's own domain but rendered by Vanta's\n    trust-report bundle (assets.vanta.com/static/vite/index-trust-report.*,\n    canonical https://trust.actively.ai, og:image https://app.vanta.com/doc?s=...).\n  slug_id: 3d4g42dma0shpytthfey2\nstatement: >-\n  \"We know that as a customer, you're entrusting us with sensitive data and we\n  take this responsibility very seriously. Security and privacy are top\n  priorities and we're committed to securing your organization's data,\n  eliminating\
  \ vulnerabilities, and ensuring continuity of access.\"\ncertifications:\n- name: SOC 2 Type II\n  scope: Security trust services category\n  cadence: audited annually\n  availability: report available on request\n  source: https://www.actively.ai/security\n- name: ISO 27001\n  scope: data center (Google Cloud facilities)\n  source: https://www.actively.ai/security\n- name: HITRUST\n  scope: data center (Google Cloud facilities)\n  source: https://www.actively.ai/security\n- name: GDPR\n  scope: data retention; DPA offered for EU customers\n  source: https://www.actively.ai/security\n- name: CCPA\n  scope: policies, processes and controls\n  source: https://www.actively.ai/security\ncontrols_published:\n- control: encryption in transit\n  detail: \"All data sent to or from Actively is encrypted using TLS.\"\n  source: https://www.actively.ai/security\n- control: encryption at rest\n  detail: >-\n    \"all customer data is encrypted using AES-256 and stored in Google\n    BigQuery.\"\n\
  \  source: https://www.actively.ai/security\n- control: physical security\n  detail: >-\n    \"All of our data in physically secure Google Cloud facilities that include\n    24/7 on-site security, camera surveillance.\"\n  source: https://www.actively.ai/security\n- control: availability / fault tolerance\n  detail: >-\n    \"Infrastructure has been designed to be fault tolerant. All databases\n    operate in a cluster configuration.\"\n  source: https://www.actively.ai/security\n- control: server hardening\n  detail: >-\n    \"All servers are configured using a documented set of security guidelines\n    and images are managed centrally.\"\n  source: https://www.actively.ai/security\n- control: subprocessors\n  detail: >-\n    \"We use secure subprocessors behind-the-scenes to connect to your\n    Salesforce and other sales software tools.\"\n  source: https://www.actively.ai/security\nsecurity_contact: security@actively.ai\ndisclosure_policy: https://www.actively.ai/responsible-disclosure\n\
  document_access: >-\n  Not machine-readable. The trust center is a client-rendered single-page\n  application; the certification list, document inventory and any NDA/request\n  gate are fetched by JavaScript from Vanta's signed GraphQL API and are not\n  present in the served HTML. The certifications recorded above are therefore\n  sourced from the company's own security page, which states them in plain\n  text.\nlimitations:\n- >-\n  trust.actively.ai returns HTTP 200 with a complete <head> (title \"Actively\n  Trust Center\", full description) but an EMPTY <body> — 5,021 bytes of\n  bootstrap. Nothing about the actual security posture is retrievable without\n  executing JavaScript.\n- >-\n  No subprocessor list, no pen-test summary, no data-residency statement and\n  no SSO/RBAC detail is published in any machine-readable form.\nevidence:\n- fetched: '2026-08-13'\n  url: https://trust.actively.ai/\n  http_status: 200\n  content_type: text/html\n  bytes: 5021\n- fetched: '2026-08-13'\n\
  \  url: https://www.actively.ai/security\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actively/refs/heads/main/security/actively-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, HITRUST, GDPR, CCPA
tags:
- Company
- Ai Apps
- AI Agents
- Revenue Intelligence
- Sales
- Go To Market
- MCP
- OAuth
- Model Context Protocol
- Sales Intelligence
- Enterprise Software
trust_url: https://trust.actively.ai/
---
