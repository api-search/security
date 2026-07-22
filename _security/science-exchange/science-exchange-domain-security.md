---
api_specs:
- filename: science-exchange-providers-openapi.yml
  format: yaml
  label: Science Exchange Providers API
  slug: science-exchange-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/science-exchange/refs/heads/main/openapi/science-exchange-providers-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scienceexchange.com
  spf: true
hosts:
- cert_expires: Sep 11 01:17:11 2026 GMT
  host: www.scienceexchange.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 15:29:45 2026 GMT
  host: demo.scienceexchange.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Science Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Science Exchange, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Science Exchange
provider_slug: science-exchange
slug: science-exchange-domain-security
source_filename: science-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scienceexchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:17:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo.scienceexchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:29:45 2026 GMT\n  hsts: null\ndomains:\n- domain: scienceexchange.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/science-exchange/refs/heads/main/security/science-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Life Sciences
- Research and Development
- Scientific Services
- Procurement
- Marketplace
- Supplier Management
- Biotech
- Pharmaceuticals
- API
---
