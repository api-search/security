---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@cequence.ai"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cequence.ai
  spf: true
hosts:
- cert_expires: Nov 24 17:51:04 2026 GMT
  host: www.cequence.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:42:47 2026 GMT
  host: helpdesk.cequence.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 17:26:13 2026 GMT
  host: docs.aigateway.cequence.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cequence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cequence Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cequence Security
provider_slug: cequence
slug: cequence-domain-security
source_filename: cequence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cequence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 17:51:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: helpdesk.cequence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:42:47 2026 GMT\n  hsts: null\n- host: docs.aigateway.cequence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 17:26:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: cequence.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@cequence.ai\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cequence/refs/heads/main/security/cequence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Protection
- API Discovery
- API Security
- Application Security
- Attack Surface
- Bot Management
- Business Logic Abuse
- CNAPP
- Cybersecurity
- Fraud
- Unified API Protection
---
