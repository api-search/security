---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: locationiq.org
  spf: true
hosts:
- cert_expires: Sep 20 12:01:58 2026 GMT
  host: locationiq.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Locationiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocationIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LocationIQ
provider_slug: locationiq
slug: locationiq-domain-security
source_filename: locationiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: locationiq.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:01:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: locationiq.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locationiq/refs/heads/main/security/locationiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Public APIs
---
