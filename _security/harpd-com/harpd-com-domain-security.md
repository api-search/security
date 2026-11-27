---
api_specs:
- filename: harpd-com-agent-api-openapi.yml
  format: yaml
  label: Harpd Agent API
  slug: harpd-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harpd-com/openapi/harpd-com-agent-api-openapi.yml
- filename: harpd-com-payments-api-openapi.yml
  format: yaml
  label: Harpd Payments API
  slug: harpd-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harpd-com/openapi/harpd-com-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: harpd.com
  spf: true
hosts:
- cert_expires: Dec 27 22:02:34 2026 GMT
  host: harpd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 16:45:54 2026 GMT
  host: api.harpd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Harpd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harpd, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Harpd
provider_slug: harpd-com
slug: harpd-com-domain-security
source_filename: harpd-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harpd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 22:02:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.harpd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 16:45:54 2026 GMT\n  hsts: false\ndomains:\n- domain: harpd.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/harpd-com/security/harpd-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Rankings
- Data
- Research
- Open Data
- Company
---
