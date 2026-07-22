---
api_specs:
- filename: sinai-technologies-openapi-original.yml
  format: yaml
  label: SINAI API
  slug: sinai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinai-technologies/refs/heads/main/openapi/sinai-technologies-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sinaitechnologies.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sinai.com
  spf: true
hosts:
- cert_expires: Oct 14 20:00:08 2026 GMT
  host: sinaitechnologies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.sinai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sinai Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sinai Technologies, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sinai Technologies
provider_slug: sinai-technologies
slug: sinai-technologies-domain-security
source_filename: sinai-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sinaitechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:00:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sinai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sinaitechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sinai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinai-technologies/refs/heads/main/security/sinai-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Carbon Management
- Carbon Accounting
- Emissions
- Sustainability
- ESG
- Decarbonization
- Climate
---
