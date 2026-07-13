---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Rentec Direct Open API
  slug: rentec-direct-api
  spec_type: OpenAPI
  url: https://secure.rentecdirect.com/api/v3/docs/
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rentecdirect.com
  spf: true
hosts:
- cert_expires: Sep 27 17:29:09 2026 GMT
  host: www.rentecdirect.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:29:09 2026 GMT
  host: secure.rentecdirect.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rentec Direct, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Rentec Direct
provider_slug: rentec
slug: rentec-domain-security
source_filename: rentec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rentecdirect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:29:09 2026 GMT\n  hsts: false\n- host: secure.rentecdirect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:29:09 2026 GMT\n  hsts: false\ndomains:\n- domain: rentecdirect.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentec/refs/heads/main/security/rentec-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Property Management
- Real Estate
- Rental
- Tenant Screening
- Payments
- Maintenance
- Financial Reporting
---
