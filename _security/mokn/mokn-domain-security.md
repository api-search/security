---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mokn.io
  spf: true
hosts:
- cert_expires: Aug 23 15:07:24 2026 GMT
  host: mokn.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mokn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MokN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MokN
provider_slug: mokn
slug: mokn-domain-security
source_filename: mokn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mokn.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:07:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mokn.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mokn/refs/heads/main/security/mokn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Cybersecurity
- Threat Detection
- Deception Technology
- Attack Surface Management
- Credential Security
---
