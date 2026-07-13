---
api_specs:
- filename: intralinks-api-openapi.yml
  format: yaml
  label: Intralinks API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: intralinks.com
  spf: true
hosts:
- host: developers.intralinks.com
  https: false
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.intralinks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intralinks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intralinks, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Intralinks
provider_slug: intralinks
slug: intralinks-domain-security
source_filename: intralinks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.intralinks.com\n  https: false\n- host: api.intralinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: intralinks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/security/intralinks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
---
