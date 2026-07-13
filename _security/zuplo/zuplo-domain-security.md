---
api_specs:
- filename: zuplo-openapi.yml
  format: yaml
  label: Zuplo Developer API
  slug: zuplo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/openapi/zuplo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zuplo.com
  spf: true
hosts:
- cert_expires: Aug 17 03:16:39 2026 GMT
  host: zuplo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 13:23:10 2026 GMT
  host: dev.zuplo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zuplo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zuplo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Zuplo
provider_slug: zuplo
slug: zuplo-domain-security
source_filename: zuplo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zuplo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 03:16:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.zuplo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 13:23:10 2026 GMT\n  hsts: null\ndomains:\n- domain: zuplo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuplo/refs/heads/main/security/zuplo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Gateway
- API Management
- Gateways
- Platform
---
