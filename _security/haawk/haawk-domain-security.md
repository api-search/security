---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: haawk.com
  spf: true
hosts:
- cert_expires: Sep  5 10:48:20 2026 GMT
  host: haawk.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Haawk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HAAWK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HAAWK
provider_slug: haawk
slug: haawk-domain-security
source_filename: haawk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haawk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 10:48:20 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: haawk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haawk/refs/heads/main/security/haawk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Rights Management
- Content ID
- Music Distribution
- Sync Licensing
- Copyright
- Media
---
