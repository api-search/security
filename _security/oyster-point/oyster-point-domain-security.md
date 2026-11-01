---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oysterpoint.com
  spf: true
hosts:
- cert_expires: Dec 14 03:19:18 2026 GMT
  host: www.oysterpoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oyster Point Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oyster Point, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Oyster Point
provider_slug: oyster-point
slug: oyster-point-domain-security
source_filename: oyster-point-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oysterpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 03:19:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oysterpoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/oyster-point/security/oyster-point-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- HealthTech
- Biotech
- DataPlatform
- VentureBacked
---
