---
api_specs:
- filename: navis-n4-openapi.yml
  format: yaml
  label: NAVIS N4 Terminal Operating System API
  slug: n4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/openapi/navis-n4-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaleris.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: navis.com
  spf: true
hosts:
- cert_expires: Sep 25 07:49:20 2026 GMT
  host: kaleris.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 07:49:20 2026 GMT
  host: www.navis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navis (Kaleris), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Navis (Kaleris)
provider_slug: navis
slug: navis-domain-security
source_filename: navis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaleris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:49:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.navis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:49:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kaleris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: navis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/security/navis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maritime
- Port
- Terminal
- Container
- Logistics
---
