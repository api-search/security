---
api_specs:
- filename: trustlayer-platform-v2-openapi.yaml
  format: yaml
  label: TrustLayer Platform API v2
  slug: trustlayer-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustlayer/refs/heads/main/openapi/trustlayer-platform-v2-openapi.yaml
- filename: trustlayer-platform-v1-openapi.yaml
  format: yaml
  label: TrustLayer Platform API v1
  slug: trustlayer-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustlayer/refs/heads/main/openapi/trustlayer-platform-v1-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trustlayer.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: trustlayer.dev
  spf: false
hosts:
- cert_expires: Sep 19 11:46:04 2026 GMT
  host: trustlayer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:51:37 2026 GMT
  host: api.trustlayer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 14:49:54 2026 GMT
  host: api.integration.trustlayer.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trustlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrustLayer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TrustLayer
provider_slug: trustlayer
slug: trustlayer-domain-security
source_filename: trustlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustlayer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:46:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.trustlayer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:51:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.integration.trustlayer.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 14:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trustlayer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: trustlayer.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustlayer/refs/heads/main/security/trustlayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Insurtech
- Insurance
- Risk Management
- Compliance
- Certificate of Insurance
- Vendor Management
---
