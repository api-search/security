---
api_specs:
- filename: utilityhouse-xyz-grants-api-openapi.yml
  format: yaml
  label: utilityhouse-xyz Grants API
  slug: utilityhouse-xyz-grants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/utilityhouse-xyz/openapi/utilityhouse-xyz-grants-api-openapi.yml
- filename: utilityhouse-xyz-woo-api-openapi.yml
  format: yaml
  label: utilityhouse-xyz Woo API
  slug: utilityhouse-xyz-woo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/utilityhouse-xyz/openapi/utilityhouse-xyz-woo-api-openapi.yml
- filename: utilityhouse-xyz-wp-updates-api-openapi.yml
  format: yaml
  label: utilityhouse-xyz Wp Updates API
  slug: utilityhouse-xyz-wp-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/utilityhouse-xyz/openapi/utilityhouse-xyz-wp-updates-api-openapi.yml
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
  dmarc_policy: none
  dnssec: true
  domain: utilityhouse.xyz
  spf: true
hosts:
- cert_expires: Jan 25 02:28:08 2027 GMT
  host: utilityhouse.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Utilityhouse Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for utilityhouse-xyz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: utilityhouse-xyz
provider_slug: utilityhouse-xyz
slug: utilityhouse-xyz-domain-security
source_filename: utilityhouse-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utilityhouse.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 02:28:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: utilityhouse.xyz\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/utilityhouse-xyz/security/utilityhouse-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Software
- Grants
- WordPress
- WooCommerce
---
