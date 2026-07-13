---
api_specs:
- filename: roku-external-control-protocol.yaml
  format: yaml
  label: Roku External Control Protocol (ECP)
  slug: external-control-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-external-control-protocol.yaml
- filename: roku-pay-web-services.yaml
  format: yaml
  label: Roku Pay Web Services
  slug: pay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-pay-web-services.yaml
- filename: roku-nabu-cloud.yaml
  format: yaml
  label: Roku Nabu Cloud
  slug: nabu-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-nabu-cloud.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roku.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roku.dev
  spf: true
hosts:
- cert_expires: Sep 15 19:27:59 2026 GMT
  host: www.roku.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: developer.roku.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: api.cloud.roku.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Roku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roku, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Roku
provider_slug: roku
slug: roku-domain-security
source_filename: roku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:27:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.roku.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.cloud.roku.dev\n  https: false\ndomains:\n- domain: roku.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: roku.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/security/roku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Streaming
- Television
- Media
- Entertainment
- Connected TV
- Consumer Electronics
---
