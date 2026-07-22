---
api_specs:
- filename: tempus-ex-fusionfeed-asyncapi.yml
  format: yaml
  label: FusionFeed
  slug: fusionfeed
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tempus-ex/refs/heads/main/asyncapi/tempus-ex-fusionfeed-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tempus-ex.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: tempus-ex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: docs.tempus-ex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 06:42:51 2026 GMT
  host: feed.fusion.tempus-ex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tempus Ex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tempus Ex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tempus Ex
provider_slug: tempus-ex
slug: tempus-ex-domain-security
source_filename: tempus-ex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tempus-ex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: docs.tempus-ex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: false\n- host: feed.fusion.tempus-ex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:42:51 2026 GMT\n  hsts: false\ndomains:\n- domain: tempus-ex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tempus-ex/refs/heads/main/security/tempus-ex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sports Data
- Sports
- Video
- Streaming
- Telemetry
- GraphQL
- REST
- Media
- NFL
- Analytics
---
