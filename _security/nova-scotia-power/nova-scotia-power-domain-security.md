---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nspower.ca
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.nspower.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:03:48 2026 GMT
  host: greenbutton.nspower.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 18:43:19 2026 GMT
  host: accounts.nspower.ca
  hsts: true
  hsts_directives: includeSubDomains; preload
  hsts_max_age: 31536000
  https: true
  note: LoginRadius-hosted customer identity provider (SAML IdP).
  tls_version: TLSv1.3
- cert_expires: Oct 19 19:43:22 2026 GMT
  host: myaccount.nspower.ca
  hsts: true
  hsts_directives: includeSubDomains; preload
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:47:21 2026 GMT
  host: oasis.nspower.ca
  hsts: null
  https: true
  note: 301s every path to https://www.nspower.ca/oasis — a vanity redirect, not a site.
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: outagemap.nspower.ca
  hsts: null
  https: true
  note: KUBRA-hosted outage map; HTTP/2, CDN-fronted.
  tls_version: TLSv1.3
- cert_expires: Sep 21 16:02:00 2026 GMT
  host: greenbuttonuat.nspower.ca
  hsts: null
  https: false
  note: A UAT environment exists and negotiates TLS, but the certificate carries no subject alternative name matching this host, so a normal client closes the connection. Not a usable public surface.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nova Scotia Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nova Scotia Power, probed live across 7 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nova Scotia Power
provider_slug: nova-scotia-power
slug: nova-scotia-power-domain-security
source_filename: nova-scotia-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nspower.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: greenbutton.nspower.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:03:48 2026 GMT\n  hsts: null\n- host: accounts.nspower.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 18:43:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_directives: includeSubDomains; preload\n  note: LoginRadius-hosted customer identity provider (SAML IdP).\n- host: myaccount.nspower.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 19:43:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_directives: includeSubDomains; preload\n- host: oasis.nspower.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:47:21 2026 GMT\n  hsts: null\n  note: >-\n    301s every\
  \ path to https://www.nspower.ca/oasis — a vanity redirect, not a site.\n- host: outagemap.nspower.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\n  note: KUBRA-hosted outage map; HTTP/2, CDN-fronted.\n- host: greenbuttonuat.nspower.ca\n  https: false\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:02:00 2026 GMT\n  hsts: null\n  note: >-\n    A UAT environment exists and negotiates TLS, but the certificate carries no\n    subject alternative name matching this host, so a normal client closes the\n    connection. Not a usable public surface.\nhosts_note: >-\n  The first two hosts were probed by 0-working/probe-domain-security.py from the\n  apis.yml properties; the remaining five were probed by hand on 2026-07-27 with the\n  same technique (TLS handshake + HTTP HEAD) to cover every Nova Scotia Power host\n  found during contract discovery.\ndomains:\n- domain: nspower.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova-scotia-power/refs/heads/main/security/nova-scotia-power-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- Utilities
- Electricity
- Energy Retailer
- Green Button
- Smart Metering
- Grid
- Renewables
- Solar
- EV Charging
- Energy Markets
- Regulation
---
