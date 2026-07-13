---
api_specs:
- filename: unkey-openapi.yml
  format: yaml
  label: Unkey API
  slug: unkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey/refs/heads/main/openapi/unkey-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unkey.com
  spf: true
hosts:
- cert_expires: Sep 11 15:58:00 2026 GMT
  host: www.unkey.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: api.unkey.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Unkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unkey, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unkey
provider_slug: unkey
slug: unkey-domain-security
source_filename: unkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:58:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.unkey.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unkey.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unkey/refs/heads/main/security/unkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Keys
- Rate Limiting
- Authentication
- Developer Platform
- Access Control
- Identity
- Analytics
---
