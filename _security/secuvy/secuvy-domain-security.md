---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: secuvy.ai
  spf: true
hosts:
- cert_expires: Aug 19 09:25:07 2026 GMT
  host: secuvy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Secuvy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secuvy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Secuvy
provider_slug: secuvy
slug: secuvy-domain-security
source_filename: secuvy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secuvy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 09:25:07 2026 GMT\n  hsts: false\ndomains:\n- domain: secuvy.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secuvy/refs/heads/main/security/secuvy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Secuvy
- Data Security
- Privacy
- PII Discovery
- DSPM
- AI Governance
- Classification
- Connectors
- Compliance
- Data Discovery
---
