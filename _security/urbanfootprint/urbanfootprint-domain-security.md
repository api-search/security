---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbanfootprint.com
  spf: true
hosts:
- cert_expires: Sep  7 23:24:24 2026 GMT
  host: urbanfootprint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbanfootprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UrbanFootprint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UrbanFootprint
provider_slug: urbanfootprint
slug: urbanfootprint-domain-security
source_filename: urbanfootprint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanfootprint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:24:24 2026 GMT\n  hsts: false\ndomains:\n- domain: urbanfootprint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanfootprint/refs/heads/main/security/urbanfootprint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate
- Geospatial
- Urban Planning
- Data
- Analytics
- Resilience
- Mapping
---
