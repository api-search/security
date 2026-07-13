---
api_specs:
- filename: swagger
  format: yaml
  label: Swimlane REST API
  slug: swimlane-rest-api
  spec_type: OpenAPI
  url: https://{your-instance}.swimlane.app/api/swagger
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swimlane.com
  spf: true
hosts:
- cert_expires: Sep 10 14:59:58 2026 GMT
  host: swimlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 22:13:10 2026 GMT
  host: docs.swimlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swimlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swimlane, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Swimlane
provider_slug: swimlane
slug: swimlane-domain-security
source_filename: swimlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swimlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:59:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.swimlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 22:13:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swimlane.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/security/swimlane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SOAR
- Security Orchestration
- Automation
- Incident Response
- Playbooks
- Case Management
- Security Operations
- Agentic AI
---
