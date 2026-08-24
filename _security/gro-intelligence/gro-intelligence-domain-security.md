---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: gro-intelligence.com
  ds_records: []
  mx: []
  risk_note: No SPF, no DMARC, no CAA and no DNSSEC on a lapsed brand that once served financial-grade agricultural intelligence to traders, insurers and lenders. With no MX and no email authentication, mail claiming to be from @gro-intelligence.com cannot be distinguished from a forgery by a receiving domain. Recorded as an observed fact about an abandoned domain, not as a criticism of an operating security program.
  spf: false
  txt_leftovers:
  - atlassian-domain-verification (stale verification record from the company's former Atlassian tenant)
hosts:
- dns: NXDOMAIN
  host: api.gro-intelligence.com
  https: false
  note: The published API host. Does not resolve.
  reachable: false
- dns: NXDOMAIN
  host: developers.gro-intelligence.com
  https: false
  note: The published developer portal. Does not resolve.
  reachable: false
- dns: NXDOMAIN
  host: app.gro-intelligence.com
  https: false
  note: The web application that issued API tokens. Does not resolve.
  reachable: false
- cert_issuer: GoDaddy TLS Intermediate CA DV - R1v1
  cert_not_after: '2027-01-21'
  cert_not_before: '2026-07-07'
  cert_san:
  - gro-intelligence.com
  cert_subject: CN=gro-intelligence.com
  host: gro-intelligence.com
  hsts: false
  hsts_max_age: null
  http_version: '1.1'
  https: true
  note: Registrar parking page. A DV certificate auto-issued by GoDaddy in July 2026 — two years after the company ceased operations — which is evidence of parking infrastructure, not of an operating service.
  reachable: true
  tls_verify: ok
kind: domain-security
layout: security
method: probed
name: Gro Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gro Intelligence, probed live across 4 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gro Intelligence
provider_slug: gro-intelligence
slug: gro-intelligence-domain-security
source_filename: gro-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: dig + TLS handshake against gro-intelligence.com, 2026-08-22\nnote: >-\n  0-working/probe-domain-security.py returned `unreachable` because the only API\n  host in apis.yml (api.gro-intelligence.com) is NXDOMAIN. These values were\n  probed by hand against the registrable domain, which still has DNS. The\n  posture is the posture of an abandoned, registrar-parked domain: a valid but\n  generic DV certificate issued by the parking provider, and no email\n  authentication of any kind.\nhosts:\n- host: api.gro-intelligence.com\n  https: false\n  reachable: false\n  dns: NXDOMAIN\n  note: The published API host. Does not resolve.\n- host: developers.gro-intelligence.com\n  https: false\n  reachable: false\n  dns: NXDOMAIN\n  note: The published developer portal. Does not resolve.\n- host: app.gro-intelligence.com\n  https: false\n  reachable: false\n  dns: NXDOMAIN\n  note: The web application that issued API tokens. Does not resolve.\n\
  - host: gro-intelligence.com\n  https: true\n  reachable: true\n  http_version: '1.1'\n  tls_verify: ok\n  cert_subject: CN=gro-intelligence.com\n  cert_issuer: GoDaddy TLS Intermediate CA DV - R1v1\n  cert_not_before: '2026-07-07'\n  cert_not_after: '2027-01-21'\n  cert_san: [gro-intelligence.com]\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    Registrar parking page. A DV certificate auto-issued by GoDaddy in July\n    2026 — two years after the company ceased operations — which is evidence of\n    parking infrastructure, not of an operating service.\ndomains:\n- domain: gro-intelligence.com\n  dnssec: false\n  ds_records: []\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  mx: []\n  txt_leftovers:\n  - atlassian-domain-verification (stale verification record from the company's former Atlassian tenant)\n  risk_note: >-\n    No SPF, no DMARC, no CAA and no DNSSEC on a lapsed brand that once served\n    financial-grade agricultural intelligence to traders, insurers\
  \ and lenders.\n    With no MX and no email authentication, mail claiming to be from\n    @gro-intelligence.com cannot be distinguished from a forgery by a receiving\n    domain. Recorded as an observed fact about an abandoned domain, not as a\n    criticism of an operating security program.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gro-intelligence/refs/heads/main/security/gro-intelligence-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Agriculture
- Climate
- Data
- Analytics
- Satellite Imagery
- Commodities
- Weather
- Food Security
- Time Series
- Defunct
---
