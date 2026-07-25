---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acturis.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acturis.ca
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: acturisgroup.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: brovada.com
  spf: true
hosts:
- cert_expires: Oct 18 19:59:13 2026 GMT
  host: www.acturis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 08:43:48 2026 GMT
  host: acturis.ca
  hsts: null
  https: true
  note: HEAD probe returned no Strict-Transport-Security header (request blocked by the host).
  tls_version: TLSv1.3
- cert_expires: Aug 28 17:41:54 2026 GMT
  host: acturisgroup.com
  hsts: null
  https: true
  note: HEAD probe returned no Strict-Transport-Security header (request blocked by the host).
  tls_version: TLSv1.3
- cert_expires: Aug 29 04:24:34 2026 GMT
  host: brovada.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acturis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acturis, probed live across 4 host(s) and 4 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Acturis
provider_slug: acturis
slug: acturis-domain-security
source_filename: acturis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + Acturis Group hosts\nnote: >-\n  The primary marketing host was probed by 0-working/probe-domain-security.py;\n  the three sibling Acturis Group hosts (Acturis Canada, Acturis Group, Brovada)\n  were probed with the same routines and added by hand because they hang off\n  ParentOrganization/related links rather than a Website/baseURL pointer. There\n  is no API host to probe — Acturis publishes no public API base URL. Absence of\n  a record (no CAA on any domain, no HSTS, DMARC p=none or absent) is recorded\n  as observed, not inferred.\nhosts:\n- host: www.acturis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 19:59:13 2026 GMT\n  hsts: false\n- host: acturis.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:43:48 2026 GMT\n  hsts: null\n  note: HEAD probe returned no Strict-Transport-Security header (request blocked by the host).\n- host: acturisgroup.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:41:54 2026 GMT\n  hsts: null\n  note: HEAD probe returned no Strict-Transport-Security header (request blocked by the host).\n- host: brovada.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:24:34 2026 GMT\n  hsts: false\ndomains:\n- domain: acturis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: acturis.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: acturisgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: brovada.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acturis/refs/heads/main/security/acturis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- United Kingdom
- Broker
- Agency Management
- Policy Administration
- Claims
- Property and Casualty
- Insurtech
- E-Trade
- MGA
---
