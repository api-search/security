---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: legalandgeneral.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: landg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: lgim.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lgamerica.com
  note: former US protection arm; weakest posture of the group (p=none, SPF ~all)
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.legalandgeneral.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: group.legalandgeneral.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 16070300
  https: true
  tls_version: TLSv1.3
- host: am.landg.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 16070300
  https: true
  tls_version: TLSv1.3
- host: fundcentres.lgim.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
- host: sandbox.legalandgeneral.com
  hsts: false
  http_status: 403
  https: true
  note: CloudFront distribution, locked down — 403 with a 27-byte body on every path
  tls_version: TLSv1.3
- host: api.lgamerica.com
  hsts: false
  http_status: 403
  https: true
  note: Azure Traffic Manager / IIS backend of the former US protection arm; no public surface
  tls_version: TLSv1.3
- host: api.landg.com
  hsts: null
  https: false
  note: A record present (194.63.117.10) but TCP/443 is filtered — no TLS handshake completes and every HTTPS request times out. Network-gated partner host.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Legal And General Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Legal & General, probed live across 7 host(s) and 4 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Legal & General
provider_slug: legal-and-general
slug: legal-and-general-domain-security
source_filename: legal-and-general-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus every Legal & General host found in DNS\nhosts:\n- host: www.legalandgeneral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: group.legalandgeneral.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 16070300\n  hsts_include_subdomains: true\n- host: am.landg.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 16070300\n  hsts_include_subdomains: true\n- host: fundcentres.lgim.com\n  https: true\n  tls_version: TLSv1.2\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n- host: sandbox.legalandgeneral.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  http_status: 403\n  note: CloudFront distribution, locked down — 403 with a 27-byte body on every path\n- host: api.lgamerica.com\n  https: true\n  tls_version: TLSv1.3\n \
  \ hsts: false\n  http_status: 403\n  note: Azure Traffic Manager / IIS backend of the former US protection arm; no public surface\n- host: api.landg.com\n  https: false\n  tls_version: null\n  hsts: null\n  note: >-\n    A record present (194.63.117.10) but TCP/443 is filtered — no TLS handshake\n    completes and every HTTPS request times out. Network-gated partner host.\ndomains:\n- domain: legalandgeneral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: landg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: reject\n- domain: lgim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: reject\n- domain: lgamerica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: former US protection arm; weakest posture of the group (p=none, SPF ~all)\nfindings:\n- All primary web hosts serve TLS 1.3\
  \ with HSTS; fundcentres.lgim.com negotiates TLS 1.2.\n- No domain in the group publishes CAA records or has DNSSEC enabled.\n- SPF and DMARC are present on all four registrable domains; the three UK domains enforce p=reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legal-and-general/refs/heads/main/security/legal-and-general-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Life Insurance
- Health Insurance
- Employee Benefits
- Pensions
- Annuities
- Asset Management
- Underwriting
- Carrier
- Brokers
- Partner Gated
- No Public API
- Design System
- Agent Skills
- Open-Source
---
