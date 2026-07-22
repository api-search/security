---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hula.earth
  spf: false
hosts:
- cert_expires: Sep 15 23:16:42 2026 GMT
  host: hula.earth
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hula Earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hula Earth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Hula Earth
provider_slug: hula-earth
slug: hula-earth-domain-security
source_filename: hula-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hula.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:16:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hula.earth\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hula-earth/refs/heads/main/security/hula-earth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biodiversity
- Environmental Monitoring
- IoT
- Satellite Imagery
- Artificial Intelligence
- Sustainability
- Conservation
- Earth Observation
- ESG
---
