---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: place.com
  spf: true
hosts:
- cert_expires: Sep  1 18:23:39 2026 GMT
  host: place.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 00:23:06 2026 GMT
  host: sso.place.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 315360000
  https: true
  note: PLACE single sign-on host (Okta custom domain); serves OIDC/OAuth discovery.
  tls_version: TLSv1.2
- cert_expires: Oct 23 23:49:13 2026 GMT
  host: hub.place.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 315360000
  https: true
  note: PLACE identity hub host (Okta custom domain); serves OIDC/OAuth discovery.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Place Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PLACE, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PLACE
provider_slug: place
slug: place-domain-security
source_filename: place-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: place.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:23:39 2026 GMT\n  hsts: false\n- host: sso.place.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 00:23:06 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n  hsts_include_subdomains: true\n  note: PLACE single sign-on host (Okta custom domain); serves OIDC/OAuth discovery.\n- host: hub.place.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:49:13 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n  hsts_include_subdomains: true\n  note: PLACE identity hub host (Okta custom domain); serves OIDC/OAuth discovery.\ndomains:\n- domain: place.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/place/refs/heads/main/security/place-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- Property Technology
- PropTech
- CRM
- Transaction Management
- Brokerage
- MLS
- Mortgage
- Title and Escrow
- Business Services
- Identity
---
