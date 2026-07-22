---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lunasonde.com
  spf: true
hosts:
- cert_expires: Oct 17 01:24:40 2026 GMT
  host: lunasonde.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lunasonde Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunasonde, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lunasonde
provider_slug: lunasonde
slug: lunasonde-domain-security
source_filename: lunasonde-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lunasonde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 01:24:40 2026 GMT\n  hsts: false\ndomains:\n- domain: lunasonde.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunasonde/refs/heads/main/security/lunasonde-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Space
- Satellite
- Earth Observation
- Geophysics
- Subsurface Imaging
- Remote Sensing
- Deep Tech
---
