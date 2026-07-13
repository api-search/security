---
api_specs:
- filename: soax-web-data-api-openapi.yml
  format: yaml
  label: SOAX Web Data API
  slug: soax-web-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soax/refs/heads/main/openapi/soax-web-data-api-openapi.yml
- filename: soax-proxy-management-api-openapi.yml
  format: yaml
  label: SOAX Proxy Management API
  slug: soax-proxy-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soax/refs/heads/main/openapi/soax-proxy-management-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soax.com
  spf: true
hosts:
- cert_expires: Aug 15 18:44:22 2026 GMT
  host: soax.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 01:56:22 2026 GMT
  host: partner.api.soax.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  6 03:12:09 2026 GMT
  host: scraping.soax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SOAX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SOAX
provider_slug: soax
slug: soax-domain-security
source_filename: soax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 18:44:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: partner.api.soax.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 01:56:22 2026 GMT\n  hsts: null\n- host: scraping.soax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 03:12:09 2026 GMT\n  hsts: null\ndomains:\n- domain: soax.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soax/refs/heads/main/security/soax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Proxy
- Web Scraping
- Residential Proxies
- Mobile Proxies
- Datacenter Proxies
- Data Extraction
- Anti-Bot Bypass
---
