---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airhelp.com
  spf: true
hosts:
- cert_expires: Oct 12 04:39:59 2026 GMT
  host: www.airhelp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airhelp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airhelp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airhelp
provider_slug: airhelp
slug: airhelp-domain-security
source_filename: airhelp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airhelp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:39:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: airhelp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airhelp/refs/heads/main/security/airhelp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Flight Compensation
- Passenger Rights
- Consumer
- Legal Tech
- Insurance
---
