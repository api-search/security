---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alethea.com
  spf: true
hosts:
- cert_expires: Aug 23 18:44:33 2026 GMT
  host: alethea.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alethea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alethea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alethea
provider_slug: alethea
slug: alethea-domain-security
source_filename: alethea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alethea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:44:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alethea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alethea/refs/heads/main/security/alethea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Threat Intelligence
- Narrative Risk
- Disinformation Detection
- Risk Management
- Reputation Management
- Cybersecurity
---
