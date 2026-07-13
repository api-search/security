---
api_specs:
- filename: upbound-openapi.yml
  format: yaml
  label: Upbound API
  slug: upbound
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbound/refs/heads/main/openapi/upbound-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: upbound.io
  spf: true
hosts:
- cert_expires: Aug 30 15:02:16 2026 GMT
  host: www.upbound.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 15:08:58 2026 GMT
  host: api.upbound.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upbound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upbound, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Upbound
provider_slug: upbound
slug: upbound-domain-security
source_filename: upbound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upbound.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:02:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.upbound.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:08:58 2026 GMT\n  hsts: null\ndomains:\n- domain: upbound.io\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upbound/refs/heads/main/security/upbound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Infrastructure
- Crossplane
- Developer Experience
- Internal Developer Platform
- Platform Engineering
---
