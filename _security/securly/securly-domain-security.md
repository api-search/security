---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: securly.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.securly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:12:44 2026 GMT
  host: docs.securly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Securly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Securly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Securly
provider_slug: securly
slug: securly-domain-security
source_filename: securly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.securly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: docs.securly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:12:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: securly.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securly/refs/heads/main/security/securly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- K-12
- Education
- EdTech
- Student Safety
- Web Filtering
- Device Management
- MDM
- Wellness Monitoring
- Rostering
- OneRoster
- Gated API
---
