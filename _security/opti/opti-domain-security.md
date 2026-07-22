---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opti.ai
  spf: true
hosts:
- cert_expires: Oct 13 15:52:24 2026 GMT
  host: opti.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Opti
provider_slug: opti
slug: opti-domain-security
source_filename: opti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opti.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 15:52:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opti.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opti/refs/heads/main/security/opti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity and Access Management
- IAM
- Identity Security
- Access Governance
- Non-Human Identity
- Agentic Identity
- Least Privilege
- Compliance
- Artificial Intelligence
---
