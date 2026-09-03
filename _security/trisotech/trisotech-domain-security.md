---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: trisotech.com
  spf: true
hosts:
- cert_expires: Oct 20 19:48:30 2026 GMT
  host: www.trisotech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 19:49:53 2026 GMT
  host: cloud.trisotech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trisotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trisotech, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Trisotech
provider_slug: trisotech
slug: trisotech-domain-security
source_filename: trisotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trisotech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 19:48:30 2026 GMT\n  hsts: false\n- host: cloud.trisotech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 19:49:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trisotech.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trisotech/refs/heads/main/security/trisotech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business Process Management
- Decision Management
- Workflow Automation
- Low Code
- BPMN
- DMN
- CMMN
- Healthcare
- FHIR
- Clinical Decision Support
- Standards
- AI Agents
- Model Context Protocol
- Enterprise Architecture
---
