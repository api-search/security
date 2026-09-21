---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airvet.com
  spf: true
hosts:
- cert_expires: Oct 25 09:28:54 2026 GMT
  host: www.airvet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airvet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airvet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Airvet
provider_slug: airvet
slug: airvet-domain-security
source_filename: airvet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airvet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 09:28:54 2026 GMT\n  hsts: null\ndomains:\n- domain: airvet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airvet/refs/heads/main/security/airvet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pet Care
- Veterinary
- Telehealth
- Employee Benefits
- Health
- Mobile App
- Pets
- Company
---
