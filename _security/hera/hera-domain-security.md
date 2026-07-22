---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hellohera.com
  spf: true
hosts:
- cert_expires: Aug 20 04:04:27 2026 GMT
  host: hellohera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hera
provider_slug: hera
slug: hera-domain-security
source_filename: hera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hellohera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:04:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hellohera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hera/refs/heads/main/security/hera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Healthcare
- HealthTech
- Elder Care
- Care Management
- Medicare
---
