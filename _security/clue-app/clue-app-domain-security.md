---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: helloclue.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: helloclue.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clue App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clue (BioWink), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clue (BioWink)
provider_slug: clue-app
slug: clue-app-domain-security
source_filename: clue-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helloclue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helloclue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clue-app/refs/heads/main/security/clue-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Femtech
- Women's Health
- Reproductive Health
- Period Tracker
- Cycle Tracking
- Fertility
- Pregnancy
- Perimenopause
- Research Data
- Consumer App
---
