---
api_specs:
- filename: obie-opendata-atm-locator-standard.json
  format: json
  label: Weatherbys Bank Open Data ATM Locator API
  slug: weatherbys-open-data-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/obie-opendata-atm-locator-standard.json
- filename: obie-opendata-branch-locator-standard.json
  format: json
  label: Weatherbys Bank Open Data Branch Locator API
  slug: weatherbys-open-data-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/obie-opendata-branch-locator-standard.json
- filename: obie-opendata-personal-current-accounts-standard.json
  format: json
  label: Weatherbys Bank Open Data Personal Current Accounts API
  slug: weatherbys-open-data-personal-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/obie-opendata-personal-current-accounts-standard.json
- filename: obie-opendata-business-current-accounts-standard.json
  format: json
  label: Weatherbys Bank Open Data Business Current Accounts API
  slug: weatherbys-open-data-business-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/obie-opendata-business-current-accounts-standard.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: weatherbys.bank
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Jan 22 11:16:23 2027 GMT
  host: www.weatherbys.bank
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.openbanking.org.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: openbanking.weatherbysbank.com
  https: false
kind: domain-security
layout: security
method: probed
name: Weatherbys Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weatherbys Bank, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Weatherbys Bank
provider_slug: weatherbys-bank
slug: weatherbys-bank-domain-security
source_filename: weatherbys-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weatherbys.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 11:16:23 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.openbanking.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: openbanking.weatherbysbank.com\n  https: false\ndomains:\n- domain: weatherbys.bank\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/security/weatherbys-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Private Banking
---
