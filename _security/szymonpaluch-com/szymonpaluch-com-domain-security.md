---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    agents: []
    checked: '2026-11-25'
    index:
    - alpn:
      - h2
      target: szymonpaluch.com
    published: true
  dnssec: true
  domain: szymonpaluch.com
  spf: true
hosts:
- cert_expires: Dec 27 12:15:51 2026 GMT
  host: szymonpaluch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Szymon Paluch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Szymon Paluch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Szymon Paluch
provider_slug: szymonpaluch-com
slug: szymonpaluch-com-domain-security
source_filename: szymonpaluch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: szymonpaluch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 12:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: szymonpaluch.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-25'\n    published: true\n    index:\n    - target: szymonpaluch.com\n      alpn:\n      - h2\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/szymonpaluch-com/security/szymonpaluch-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Consulting
- AI Implementation
- Workshops
- Training
- Speaking
- Enterprise AI
- AI Strategy
---
