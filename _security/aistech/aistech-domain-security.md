---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aistechspace.com
  spf: true
hosts:
- cert_expires: Oct 30 07:55:50 2026 GMT
  host: aistechspace.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aistech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aistech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aistech
provider_slug: aistech
slug: aistech-domain-security
source_filename: aistech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aistechspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 07:55:50 2026 GMT\n  hsts: null\ndomains:\n- domain: aistechspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aistech/refs/heads/main/security/aistech-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Space
- Satellite
- Thermal Imagery
- Geospatial Intelligence
---
