---
api_specs:
- filename: charityapi-openapi.yml
  format: yaml
  label: CharityAPI
  slug: charityapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charityapi/refs/heads/main/openapi/charityapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: charityapi.org
  spf: false
hosts:
- cert_expires: Aug 15 18:11:57 2026 GMT
  host: www.charityapi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 02:27:08 2026 GMT
  host: charityapi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 23:07:04 2026 GMT
  host: api.charityapi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charityapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CharityAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CharityAPI
provider_slug: charityapi
slug: charityapi-domain-security
source_filename: charityapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charityapi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 18:11:57 2026 GMT\n  hsts: false\n- host: charityapi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 02:27:08 2026 GMT\n  hsts: false\n- host: api.charityapi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:07:04 2026 GMT\n  hsts: false\ndomains:\n- domain: charityapi.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charityapi/refs/heads/main/security/charityapi-domain-security.yml
summary_line: TLSv1.3
tags:
- 501c3
- Charities
- Donations
- EIN
- IRS
- Non-Profits
- Tax Compliance
- Verification
---
