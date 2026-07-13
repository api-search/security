---
api_specs:
- filename: vehicle-history-api
  format: yaml
  label: VINaudit Vehicle History API
  slug: vinaudit-vehicle-history-api
  spec_type: OpenAPI
  url: https://www.vinaudit.com/vehicle-history-api
- filename: vinaudit-vehicle-specifications-openapi.yml
  format: yaml
  label: VINaudit Vehicle Specifications API
  slug: vinaudit-vehicle-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-vehicle-specifications-openapi.yml
- filename: vinaudit-vehicle-market-value-openapi.yml
  format: yaml
  label: VINaudit Vehicle Market Value API
  slug: vinaudit-vehicle-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-vehicle-market-value-openapi.yml
- filename: vinaudit-vehicle-ownership-cost-openapi.yml
  format: yaml
  label: VINaudit Vehicle Ownership Cost API
  slug: vinaudit-vehicle-ownership-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-vehicle-ownership-cost-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vinaudit.com
  spf: true
hosts:
- cert_expires: Sep 24 00:02:35 2026 GMT
  host: www.vinaudit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 00:02:35 2026 GMT
  host: api.vinaudit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 00:02:35 2026 GMT
  host: specifications.vinaudit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vinaudit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VINaudit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VINaudit
provider_slug: vinaudit
slug: vinaudit-domain-security
source_filename: vinaudit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vinaudit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:02:35 2026 GMT\n  hsts: false\n- host: api.vinaudit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:02:35 2026 GMT\n  hsts: false\n- host: specifications.vinaudit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:02:35 2026 GMT\n  hsts: false\ndomains:\n- domain: vinaudit.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/security/vinaudit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vehicle History
- VIN Decoding
- Automotive
- NMVTIS
- Vehicle Specifications
- Market Value
- Recall Data
- REST
---
