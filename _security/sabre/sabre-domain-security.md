---
api_specs:
- filename: sabre-bargain-finder-max-openapi.yml
  format: yaml
  label: Sabre Bargain Finder Max API
  slug: bargain-finder-max
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sabre/refs/heads/main/openapi/sabre-bargain-finder-max-openapi.yml
- filename: sabre-hotels-openapi.yml
  format: yaml
  label: Sabre Hotels API
  slug: hotels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sabre/refs/heads/main/openapi/sabre-hotels-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sabre.com
  spf: true
hosts:
- cert_expires: Sep  3 09:39:52 2026 GMT
  host: developer.sabre.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 09:39:52 2026 GMT
  host: www.sabre.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.sabre.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sabre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sabre, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sabre
provider_slug: sabre
slug: sabre-domain-security
source_filename: sabre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.sabre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:39:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.sabre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:39:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sabre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sabre.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sabre/refs/heads/main/security/sabre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- GDS
- Airlines
- Hotels
- Car Rental
- Booking
---
