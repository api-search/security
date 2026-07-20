---
api_specs:
- filename: griffin-openapi-original.yml
  format: yaml
  label: The Griffin API
  slug: the-griffin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/griffin/refs/heads/main/openapi/griffin-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: griffin.sh
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: griffin.com
  spf: true
hosts:
- host: griffin.sh
  https: false
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.griffin.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Griffin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Griffin, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Griffin
provider_slug: griffin
slug: griffin-domain-security
source_filename: griffin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: griffin.sh\n  https: false\n- host: api.griffin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: griffin.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: griffin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/griffin/refs/heads/main/security/griffin-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- Banking
- Banking as a Service
- Payments
- KYC
- Open Banking
- Bank Accounts
- Financial Services
---
