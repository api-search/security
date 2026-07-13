---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "globalsign.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: epexspot.com
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.epexspot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epex Spot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EPEX SPOT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EPEX SPOT
provider_slug: epex-spot
slug: epex-spot-domain-security
source_filename: epex-spot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epexspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: epexspot.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epex-spot/refs/heads/main/security/epex-spot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Day-Ahead Prices
- Electricity
- Energy Markets
- Power Exchange
- Intraday Trading
- Market Data
- Auctions
- Europe
---
