---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mindoktor.se
  spf: true
hosts:
- cert_expires: Oct 15 15:03:45 2026 GMT
  host: www.mindoktor.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Min Doktor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Min Doktor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Min Doktor
provider_slug: min-doktor
slug: min-doktor-domain-security
source_filename: min-doktor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mindoktor.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mindoktor.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/min-doktor/refs/heads/main/security/min-doktor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Tech
- Telemedicine
- Digital Health
- Primary Care
- Healthcare
- Sweden
---
