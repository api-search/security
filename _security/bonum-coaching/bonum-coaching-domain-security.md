---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bonumcoaching.com
  spf: true
hosts:
- cert_expires: Oct  3 06:30:28 2026 GMT
  host: bonumcoaching.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bonum Coaching Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonum Coaching, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bonum Coaching
provider_slug: bonum-coaching
slug: bonum-coaching-domain-security
source_filename: bonum-coaching-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bonumcoaching.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:30:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bonumcoaching.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonum-coaching/refs/heads/main/security/bonum-coaching-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coaching
- Human Resources
- Talent Development
- Leadership
- Mentoring
- Artificial Intelligence
- Enterprise
---
