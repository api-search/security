---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gouv.fr
  spf: false
hosts:
- cert_expires: Sep  4 07:53:15 2026 GMT
  host: adresse.data.gouv.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adresse Data Gouv Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for adresse.data.gouv.fr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: adresse.data.gouv.fr
provider_slug: adresse-data-gouv-fr
slug: adresse-data-gouv-fr-domain-security
source_filename: adresse-data-gouv-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adresse.data.gouv.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 07:53:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gouv.fr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adresse-data-gouv-fr/refs/heads/main/security/adresse-data-gouv-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Public APIs
---
