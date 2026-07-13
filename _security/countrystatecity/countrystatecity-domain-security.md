---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: countrystatecity.in
  spf: true
hosts:
- cert_expires: Aug 13 01:14:25 2026 GMT
  host: countrystatecity.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Countrystatecity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CountryStateCity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CountryStateCity
provider_slug: countrystatecity
slug: countrystatecity-domain-security
source_filename: countrystatecity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: countrystatecity.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:14:25 2026 GMT\n  hsts: false\ndomains:\n- domain: countrystatecity.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/countrystatecity/refs/heads/main/security/countrystatecity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geocoding
- Public APIs
---
