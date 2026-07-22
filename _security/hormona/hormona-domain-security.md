---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hormona.io
  spf: true
hosts:
- cert_expires: Oct  8 19:19:34 2026 GMT
  host: hormona.io
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hormona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hormona, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hormona
provider_slug: hormona
slug: hormona-domain-security
source_filename: hormona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hormona.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hormona.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hormona/refs/heads/main/security/hormona-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Femtech
- Women's Health
- Hormones
- Wellness
- Consumer Health
- Mobile App
---
