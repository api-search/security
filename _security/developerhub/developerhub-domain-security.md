---
api_specs:
- filename: developerhub-openapi.yml
  format: yaml
  label: DeveloperHub Documentation Platform
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: developerhub.io
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: developerhub.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 11:21:20 2026 GMT
  host: api.developerhub.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Developerhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeveloperHub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DeveloperHub
provider_slug: developerhub
slug: developerhub-domain-security
source_filename: developerhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developerhub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: false\n- host: api.developerhub.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 17 11:21:20 2026 GMT\n  hsts: false\ndomains:\n- domain: developerhub.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/security/developerhub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Reference
- Developer Portals
- Documentation
- Knowledge Base
---
