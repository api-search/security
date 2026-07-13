---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: councils.gov
  spf: true
hosts:
- cert_expires: Aug 13 12:21:19 2026 GMT
  host: www.councils.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chief Information Officers Council Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chief Information Officers Council, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chief Information Officers Council
provider_slug: chief-information-officers-council
slug: chief-information-officers-council-domain-security
source_filename: chief-information-officers-council-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.councils.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 12:21:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: councils.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chief-information-officers-council/refs/heads/main/security/chief-information-officers-council-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CIO
- Cloud
- Cybersecurity
- E-Government
- Federal Government
- IT Modernization
- Information Technology
- Interagency Council
- OMB
- Public Sector
---
