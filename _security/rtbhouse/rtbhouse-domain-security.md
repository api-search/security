---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: RTB House Client Panel API
  slug: rtb-house-client-panel-api
  spec_type: OpenAPI
  url: https://api.panel.rtbhouse.com/api/docs/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rtbhouse.com
  spf: true
hosts:
- cert_expires: Sep 26 19:45:38 2026 GMT
  host: www.rtbhouse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:17:07 2026 GMT
  host: api.panel.rtbhouse.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rtbhouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RTB House, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RTB House
provider_slug: rtbhouse
slug: rtbhouse-domain-security
source_filename: rtbhouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rtbhouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:45:38 2026 GMT\n  hsts: false\n- host: api.panel.rtbhouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:17:07 2026 GMT\n  hsts: null\ndomains:\n- domain: rtbhouse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/security/rtbhouse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Retargeting
- Programmatic
- DSP
- Deep Learning
- RTB
- Performance Marketing
---
