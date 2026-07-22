---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: concertocare.com
  spf: true
hosts:
- cert_expires: Aug 29 13:13:45 2026 GMT
  host: concertocare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Concertocare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConcertoCare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ConcertoCare
provider_slug: concertocare
slug: concertocare-domain-security
source_filename: concertocare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: concertocare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 13:13:45 2026 GMT\n  hsts: false\ndomains:\n- domain: concertocare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concertocare/refs/heads/main/security/concertocare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Home Health
- Senior Care
- Primary Care
- Value-Based Care
- Medicare
- Palliative Care
- Telehealth
---
