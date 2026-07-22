---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pilot.com
  spf: true
hosts:
- cert_expires: Sep 13 03:53:46 2026 GMT
  host: pilot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pilot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pilot
provider_slug: pilot
slug: pilot-domain-security
source_filename: pilot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:53:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pilot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pilot/refs/heads/main/security/pilot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Accounting
- Bookkeeping
- Tax
- CFO Services
- Startups
- Finance
---
