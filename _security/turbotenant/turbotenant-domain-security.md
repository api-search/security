---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: turbotenant.com
  spf: true
hosts:
- cert_expires: Aug 16 19:28:53 2026 GMT
  host: www.turbotenant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 17:53:20 2026 GMT
  host: api.turbotenant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turbotenant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TurboTenant, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TurboTenant
provider_slug: turbotenant
slug: turbotenant-domain-security
source_filename: turbotenant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.turbotenant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 19:28:53 2026 GMT\n  hsts: false\n- host: api.turbotenant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:53:20 2026 GMT\n  hsts: false\ndomains:\n- domain: turbotenant.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turbotenant/refs/heads/main/security/turbotenant-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Property Management
- Rental Listings
- Tenant Screening
- Rent Collection
- Lease Agreements
- Maintenance Requests
- Real Estate
---
