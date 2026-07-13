---
api_specs:
- filename: liberty-mutual-insurance-renters-insurance-api-openapi.yml
  format: yaml
  label: Liberty Mutual Renters Insurance API
  slug: renters-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-mutual-insurance/refs/heads/main/openapi/liberty-mutual-insurance-renters-insurance-api-openapi.yml
- filename: liberty-mutual-insurance-solaria-labs-api-openapi.yml
  format: yaml
  label: Liberty Mutual Solaria Labs API
  slug: solaria-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-mutual-insurance/refs/heads/main/openapi/liberty-mutual-insurance-solaria-labs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: libertymutual.com
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: www.libertymutual.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.libertymutual.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: developer.libertymutual.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liberty Mutual Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liberty Mutual Insurance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Liberty Mutual Insurance
provider_slug: liberty-mutual-insurance
slug: liberty-mutual-insurance-domain-security
source_filename: liberty-mutual-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.libertymutual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.libertymutual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\n- host: developer.libertymutual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: libertymutual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liberty-mutual-insurance/refs/heads/main/security/liberty-mutual-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Casualty
- Commercial Lines
- Insurance
- Personal Lines
- Property
- Renters
- Safety Data
- Fortune 100
---
