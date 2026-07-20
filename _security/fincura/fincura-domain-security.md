---
api_specs:
- filename: fincura-openapi-original.yml
  format: yaml
  label: Automated Spreading and Analysis API
  slug: automated-spreading-and-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincura/refs/heads/main/openapi/fincura-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abrigo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fincura.com
  spf: true
hosts:
- cert_expires: Sep 14 09:11:22 2026 GMT
  host: www.abrigo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: api.fincura.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fincura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fincura, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fincura
provider_slug: fincura
slug: fincura-domain-security
source_filename: fincura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abrigo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:11:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fincura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abrigo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fincura.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fincura/refs/heads/main/security/fincura-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Lending
- Credit Analysis
- Financial Spreading
- Banking
- Fintech
- Underwriting
- Company
---
