---
api_specs:
- filename: mettle-open-data-api-openapi.json
  format: json
  label: Mettle Open Data Product API
  slug: mettle-open-data-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mettle/refs/heads/main/openapi/mettle-open-data-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mettle.co.uk
  spf: true
- caa:
  - 0 iodef "mailto:RBS.Group.PKI.Certificates@rbs.co.uk"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bankofapis.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.mettle.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.bankofapis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: api.openbanking.prd-mettle.co.uk
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Mettle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mettle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mettle
provider_slug: mettle
slug: mettle-domain-security
source_filename: mettle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mettle.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bankofapis.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openbanking.prd-mettle.co.uk\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: mettle.co.uk\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bankofapis.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:RBS.Group.PKI.Certificates@rbs.co.uk\"\
  \n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mettle/refs/heads/main/security/mettle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Business Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
---
