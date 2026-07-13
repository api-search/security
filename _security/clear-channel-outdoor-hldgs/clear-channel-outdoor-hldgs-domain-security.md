---
api_specs:
- filename: clear-channel-outdoor-direct-openapi.yml
  format: yaml
  label: Clear Channel Outdoor Automated Direct API
  slug: clear-channel-outdoor-direct
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-channel-outdoor-hldgs/refs/heads/main/openapi/clear-channel-outdoor-direct-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clearchanneloutdoor.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cco.io
  spf: true
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: www.clearchanneloutdoor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 02:42:15 2026 GMT
  host: developer.cco.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: direct.cco.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clear Channel Outdoor Hldgs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clear Channel Outdoor Holdings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clear Channel Outdoor Holdings
provider_slug: clear-channel-outdoor-hldgs
slug: clear-channel-outdoor-hldgs-domain-security
source_filename: clear-channel-outdoor-hldgs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearchanneloutdoor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: false\n- host: developer.cco.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:42:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: direct.cco.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: clearchanneloutdoor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cco.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear-channel-outdoor-hldgs/refs/heads/main/security/clear-channel-outdoor-hldgs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Out Of Home
- Programmatic
- Digital Out Of Home
- pDOOH
- OpenRTB
- OpenDirect
---
