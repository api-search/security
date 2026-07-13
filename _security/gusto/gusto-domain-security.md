---
api_specs:
- filename: gusto-asyncapi.yml
  format: yaml
  label: Gusto Embedded Payroll API
  slug: embedded-payroll-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gusto.com
  spf: true
hosts:
- cert_expires: Oct  7 01:59:03 2026 GMT
  host: gusto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 02:36:55 2026 GMT
  host: docs.gusto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 15:33:13 2026 GMT
  host: api.gusto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gusto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gusto, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gusto
provider_slug: gusto
slug: gusto-domain-security
source_filename: gusto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gusto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:59:03 2026 GMT\n  hsts: null\n- host: docs.gusto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:36:55 2026 GMT\n  hsts: null\n- host: api.gusto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:33:13 2026 GMT\n  hsts: null\ndomains:\n- domain: gusto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/security/gusto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Human Resources
- Payroll
- Benefits
- Enterprise Software
- Embedded Finance
---
