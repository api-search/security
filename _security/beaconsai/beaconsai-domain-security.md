---
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beacons.ai
  security_txt: false
  security_txt_note: /.well-known/security.txt returns 404 on beacons.ai and account.beacons.ai; no vulnerability disclosure program was found.
  spf: true
hosts:
- cert_expires: Oct  6 12:13:16 2026 GMT
  host: beacons.ai
  hsts: true
  hsts_header: max-age=15552000; includeSubDomains; preload
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_note: Observed directly on GET https://beacons.ai/ and https://beacons.ai/llms.txt on 2026-08-13. The automated probe reports null here because the root answers a Cloudflare 403 bot challenge to non-browser user agents; the header is present on that response and on every 200.
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beaconsai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beacons.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beacons.ai
provider_slug: beaconsai
slug: beaconsai-domain-security
source_filename: beaconsai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + MCP hosts\nhosts:\n- host: beacons.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:13:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  hsts_header: max-age=15552000; includeSubDomains; preload\n  hsts_note: >-\n    Observed directly on GET https://beacons.ai/ and https://beacons.ai/llms.txt on\n    2026-08-13. The automated probe reports null here because the root answers a\n    Cloudflare 403 bot challenge to non-browser user agents; the header is present\n    on that response and on every 200.\ndomains:\n- domain: beacons.ai\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\
  \n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  security_txt: false\n  security_txt_note: /.well-known/security.txt returns 404 on beacons.ai and\n    account.beacons.ai; no vulnerability disclosure program was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconsai/refs/heads/main/security/beaconsai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Economy
- Link in Bio
- Creator Website Builder
- Creator Storefront
- Media Kit
- Email Marketing
- Affiliate Marketing
- Creator Monetization
- Influencer Software
- MCP
- Agent Native
---
