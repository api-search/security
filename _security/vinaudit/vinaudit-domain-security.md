---
api_specs:
- filename: vinaudit-getownershipcost-php-api-openapi.yml
  format: yaml
  label: VINaudit Getownershipcost.php API
  slug: vinaudit-getownershipcost-php-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-getownershipcost-php-api-openapi.yml
- filename: vinaudit-marketvalue-api-openapi.yml
  format: yaml
  label: VINaudit Marketvalue API
  slug: vinaudit-marketvalue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-marketvalue-api-openapi.yml
- filename: vinaudit-pullreport-api-openapi.yml
  format: yaml
  label: VINaudit Pullreport API
  slug: vinaudit-pullreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-pullreport-api-openapi.yml
- filename: vinaudit-query-api-openapi.yml
  format: yaml
  label: VINaudit Query API
  slug: vinaudit-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-query-api-openapi.yml
- filename: vinaudit-report-api-openapi.yml
  format: yaml
  label: VINaudit Report API
  slug: vinaudit-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-report-api-openapi.yml
- filename: vinaudit-selections-api-openapi.yml
  format: yaml
  label: VINaudit Selections API
  slug: vinaudit-selections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-selections-api-openapi.yml
- filename: vinaudit-specifications-api-openapi.yml
  format: yaml
  label: VINaudit Specifications API
  slug: vinaudit-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-specifications-api-openapi.yml
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
