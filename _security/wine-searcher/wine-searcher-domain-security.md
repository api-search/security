---
api_specs:
- filename: wine-searcher-openapi.yml
  format: yaml
  label: Wine-Searcher API
  slug: wine-searcher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wine-searcher/refs/heads/main/openapi/wine-searcher-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "www.digicert.com"
  - 0 issuewild "www.digicert.com"
  - 0 iodef "mailto:infrastructure-team@wine-searcher.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wine-searcher.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.wine-searcher.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wine Searcher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wine-Searcher, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wine-Searcher
provider_slug: wine-searcher
slug: wine-searcher-domain-security
source_filename: wine-searcher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wine-searcher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wine-searcher.com\n  dnssec: false\n  caa:\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \"www.digicert.com\"\n  - 0 iodef \"mailto:infrastructure-team@wine-searcher.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wine-searcher/refs/heads/main/security/wine-searcher-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Marketplace
- Wine
- Prices
- Merchants
- Vintages
- Critics
---
