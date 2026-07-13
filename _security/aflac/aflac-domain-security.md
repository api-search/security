---
api_specs:
- filename: aflac-enterprise-connect-openapi.yml
  format: yaml
  label: Aflac Enterprise Connect API
  slug: enterprise-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-enterprise-connect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aflac.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: docs.enterprise-connect.aflac.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 22:04:53 2026 GMT
  host: www.aflac.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.enterprise-connect.aflac.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aflac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aflac, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: aflac
provider_slug: aflac
slug: aflac-domain-security
source_filename: aflac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.enterprise-connect.aflac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.aflac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:04:53 2026 GMT\n  hsts: null\n- host: api.enterprise-connect.aflac.com\n  https: false\ndomains:\n- domain: aflac.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/security/aflac-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
---
