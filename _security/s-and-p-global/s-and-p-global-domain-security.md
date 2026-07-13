---
api_specs:
- filename: servicecatalog
  format: yaml
  label: S&P Global Commodity Insights API
  slug: commodity-insights
  spec_type: OpenAPI
  url: https://developer.spglobal.com/commodityinsights/servicecatalog
- filename: s-and-p-global-kensho-link-openapi.yml
  format: yaml
  label: Kensho Link API
  slug: kensho-link
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s-and-p-global/refs/heads/main/openapi/s-and-p-global-kensho-link-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: platts.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.spglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: developer.spglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.platts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: S And P Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for S&P Global, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: S&P Global
provider_slug: s-and-p-global
slug: s-and-p-global-domain-security
source_filename: s-and-p-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\n- host: developer.spglobal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\n- host: api.platts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: spglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: platts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s-and-p-global/refs/heads/main/security/s-and-p-global-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Data
- Credit Ratings
- Market Intelligence
- Commodity Insights
- Energy Markets
- Capital Markets
- Fortune 500
---
