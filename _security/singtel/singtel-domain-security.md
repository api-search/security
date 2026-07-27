---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: singtel.com
  spf: true
hosts:
- cert_expires: Oct 21 18:24:22 2026 GMT
  host: www.singtel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Singtel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Singtel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Singtel
provider_slug: singtel
slug: singtel-domain-security
source_filename: singtel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.singtel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 18:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: singtel.com\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singtel/refs/heads/main/security/singtel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- Singapore
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Anti-Fraud
- CPaaS
- Messaging
- Voice
- IoT
- 5G
- Edge Computing
- Aduna
- Partner Gated
---
