---
api_specs:
- filename: xe-currency-data-api-openapi.json
  format: json
  label: Xe Currency Data API
  slug: xe-currency-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xe-currency-data-api-openapi.json
- filename: xe-payments-api-openapi.json
  format: json
  label: Xe Payments API
  slug: xe-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xe-payments-api-openapi.json
- filename: xe-mass-payments-api-openapi.json
  format: json
  label: Xe Mass Payments API
  slug: xe-mass-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xe-mass-payments-api-openapi.json
- filename: xe-currency-data-tradable-rates-api-openapi.json
  format: json
  label: Xe Currency Data Tradable Rates API
  slug: xe-currency-data-tradable-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xe-currency-data-tradable-rates-api-openapi.json
- filename: xeta-api-openapi.json
  format: json
  label: XETA API
  slug: xeta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/openapi/xeta-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue ";"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: euronet.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xe.com
  spf: true
hosts:
- cert_expires: Oct 14 09:33:17 2026 GMT
  host: www.euronet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: xecdapi.xe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.xe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Euronet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Euronet Worldwide, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Euronet Worldwide
provider_slug: euronet
slug: euronet-domain-security
source_filename: euronet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.euronet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:33:17 2026 GMT\n  hsts: false\n- host: xecdapi.xe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: null\n- host: www.xe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: euronet.com\n  dnssec: false\n  caa:\n  - 0 issue \";\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: xe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/euronet/refs/heads/main/security/euronet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- United States
- Payment Processing
- Cross-Border
- Money Transfer
- Currency Exchange
- FX
- Payouts
- Real-Time Payments
- ISO 20022
- Acquiring
---
