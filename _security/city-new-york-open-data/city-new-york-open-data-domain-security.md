---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cityofnewyork.us
  spf: false
hosts:
- cert_expires: Sep 14 02:32:33 2026 GMT
  host: opendata.cityofnewyork.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City New York Open Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City, New York Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: City, New York Open Data
provider_slug: city-new-york-open-data
slug: city-new-york-open-data-domain-security
source_filename: city-new-york-open-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.cityofnewyork.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:32:33 2026 GMT\n  hsts: false\ndomains:\n- domain: cityofnewyork.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-new-york-open-data/refs/heads/main/security/city-new-york-open-data-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Public APIs
---
