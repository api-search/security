---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: securiti.ai
  spf: true
hosts:
- cert_expires: Sep 12 03:49:41 2026 GMT
  host: securiti.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Securiti Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Securiti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Securiti
provider_slug: securiti-ai
slug: securiti-ai-domain-security
source_filename: securiti-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: securiti.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:49:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: securiti.ai\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securiti-ai/refs/heads/main/security/securiti-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Security
- Data Privacy
- AI Governance
- AI Security
- DSPM
- Data Command Center
- Data Command Graph
- Sensitive Data Intelligence
- Data Subject Requests
- DSR Automation
- Consent Management
- Universal Consent
- Mobile Consent
- Data Discovery
- Data Classification
- Data Mapping
- Data Catalog
- Data Lineage
- Data Quality
- Compliance Management
- GDPR
- CCPA
- LGPD
- PIPL
- EU AI Act
- Privacy Operations
- Gencore AI
- Agent Commander
- LLM Firewalls
- Vector Databases
- Knowledge Graph
- Connectors
- Hybrid Multicloud
---
