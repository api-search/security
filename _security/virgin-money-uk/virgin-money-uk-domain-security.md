---
api_specs:
- filename: obie-opendata-api-standard-openapi.json
  format: json
  label: Virgin Money UK Open Data API
  slug: open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/openapi/obie-opendata-api-standard-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "entrust.net"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: virginmoney.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:iodef.report@cybg.com"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cybservices.co.uk
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: uk.virginmoney.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: developer.virginmoney.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: api-ib.cybservices.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virgin Money Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virgin Money UK, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Virgin Money UK
provider_slug: virgin-money-uk
slug: virgin-money-uk-domain-security
source_filename: virgin-money-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uk.virginmoney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.virginmoney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-ib.cybservices.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: virginmoney.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cybservices.co.uk\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"sectigo.com\"\
  \n  - 0 iodef \"mailto:iodef.report@cybg.com\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/security/virgin-money-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- FAPI
---
