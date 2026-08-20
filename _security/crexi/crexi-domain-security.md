---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crexi.com
  spf: true
hosts:
- cert_expires: Sep  6 18:50:38 2026 GMT
  host: www.crexi.com
  hsts: false
  https: true
  note: Every request is answered with an HTTP 403 Cloudflare bot-management interstitial unless the client solves the challenge; no Strict-Transport-Security header is returned on that response.
  tls_version: TLSv1.3
- cert_expires: Sep  6 18:50:38 2026 GMT
  host: api.crexi.com
  hsts: false
  https: true
  note: 301 to index.html then 200; no Strict-Transport-Security header on either response. /health also returns 200 without HSTS.
  tls_version: TLSv1.3
- cert_expires: Sep  6 18:50:38 2026 GMT
  host: exchange.crexi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 12:46:21 2026 GMT
  host: api-docs.crexi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Theneo-hosted documentation portal behind an AWS ELB.
  tls_version: TLSv1.3
- host: learn.crexi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: HubSpot-hosted help centre.
- host: status.crexi.com
  hsts: true
  hsts_max_age: 259200
  https: true
  note: Atlassian Statuspage.
kind: domain-security
layout: security
method: probed
name: Crexi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CREXi, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CREXi
provider_slug: crexi
slug: crexi-domain-security
source_filename: crexi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + discovery hosts\ntooling: 0-working/probe-domain-security.py, plus a manual per-host HSTS re-probe —\n  the script's default user agent is refused by the Cloudflare and AWS ELB edges in\n  front of www.crexi.com and api-docs.crexi.com, which suppressed their response headers\n  and left hsts null\nhosts:\n- host: www.crexi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:50:38 2026 GMT\n  hsts: false\n  note: Every request is answered with an HTTP 403 Cloudflare bot-management interstitial\n    unless the client solves the challenge; no Strict-Transport-Security header is\n    returned on that response.\n- host: api.crexi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:50:38 2026 GMT\n  hsts: false\n  note: 301 to index.html then 200; no Strict-Transport-Security header on either response.\n    /health also returns 200 without HSTS.\n- host: exchange.crexi.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:50:38 2026 GMT\n  hsts: false\n- host: api-docs.crexi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 12:46:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Theneo-hosted documentation portal behind an AWS ELB.\n- host: learn.crexi.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  note: HubSpot-hosted help centre.\n- host: status.crexi.com\n  https: true\n  hsts: true\n  hsts_max_age: 259200\n  note: Atlassian Statuspage.\ndomains:\n- domain: crexi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nsummary:\n  https_everywhere: true\n  tls13_everywhere: true\n  hsts_on_primary_hosts:\
  \ false\n  hsts_note: Neither the marketplace host (www.crexi.com) nor either API host (api.crexi.com,\n    exchange.crexi.com) sets Strict-Transport-Security. HSTS is present only on the\n    three third-party-hosted properties — the Theneo docs portal, the HubSpot help\n    centre and the Atlassian status page.\n  dnssec: false\n  caa_present: true\n  spf: true\n  dmarc_enforced: true\nx-evidence:\n  fetched: '2026-08-01'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crexi/refs/heads/main/security/crexi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Commercial Real Estate
- Marketplace
- Property Data
- Listings
- Auctions
- Market Intelligence
- Data Syndication
- RESO
- Company
---
