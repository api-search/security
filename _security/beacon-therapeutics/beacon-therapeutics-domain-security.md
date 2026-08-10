---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: beacontx.com
  spf: true
hosts:
- cert_expires: Oct  4 04:42:17 2026 GMT
  host: www.beacontx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beacon Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beacon Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Beacon Therapeutics
provider_slug: beacon-therapeutics
slug: beacon-therapeutics-domain-security
source_filename: beacon-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beacontx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:42:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beacontx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beacon-therapeutics/refs/heads/main/security/beacon-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Gene Therapy
- Ophthalmology
- Clinical Trials
- Life Sciences
- Rare Disease
- Pharmaceuticals
---
