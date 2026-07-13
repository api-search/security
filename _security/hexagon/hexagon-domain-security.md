---
api_specs:
- filename: developerportal
  format: yaml
  label: Hexagon Nexus API
  slug: nexus-api
  spec_type: OpenAPI
  url: https://nexus.hexagon.com/developerportal
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hexagon.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hexagonali.com
  spf: false
hosts:
- cert_expires: Aug 17 05:25:15 2026 GMT
  host: hexagon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: nexus.hexagon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 23:59:59 2026 GMT
  host: docs.hexagonali.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hexagon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hexagon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hexagon
provider_slug: hexagon
slug: hexagon-domain-security
source_filename: hexagon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hexagon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 05:25:15 2026 GMT\n  hsts: null\n- host: nexus.hexagon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\n- host: docs.hexagonali.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hexagon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hexagonali.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexagon/refs/heads/main/security/hexagon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- Metrology
- Quality Inspection
- Digital Factory
- Production Monitoring
- Industrial IoT
- Smart Manufacturing
---
