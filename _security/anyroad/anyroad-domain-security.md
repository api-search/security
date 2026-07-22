---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anyroad.com
  spf: true
hosts:
- cert_expires: Oct  3 01:45:57 2026 GMT
  host: anyroad.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anyroad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anyroad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anyroad
provider_slug: anyroad
slug: anyroad-domain-security
source_filename: anyroad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anyroad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:45:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anyroad.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyroad/refs/heads/main/security/anyroad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Experiential Marketing
- Events
- Experiences
- Ticketing
- Consumer Engagement
- Analytics
- Webhooks
---
