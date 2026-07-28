---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blinkcharging.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: blinknetwork.com
  spf: true
  spf_all: +all
  spf_record: v=spf1 a mx include:spf.protection.outlook.com include:mail.zendesk.com a:blinknetwork.com a:smtp.blinknetwork.com a:dmz.blinknetwork.com ip4:206.225.165.104 ip4:72.44.248.138 include:amazonses.com +all
  spf_weakness: The SPF record ends in `+all`, which explicitly passes every sender and so neutralises SPF for blinknetwork.com - the domain carrying the API gateway and both host portals.
hosts:
- cert_expires: Sep 18 05:04:42 2026 GMT
  host: blinkcharging.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 12:51:03 2027 GMT
  host: api.blinknetwork.com
  hsts: false
  https: true
  note: Public Kong API gateway. No Strict-Transport-Security header on any response.
  server: kong/2.8.1
  tls_version: TLSv1.3
- cert_expires: Feb 13 12:51:03 2027 GMT
  host: host.blinknetwork.com
  hsts: false
  https: true
  note: Blink Network host portal (React SPA on S3/CloudFront). No HSTS.
  server: AmazonS3
  tls_version: TLSv1.3
- cert_expires: Feb 13 12:51:03 2027 GMT
  host: blinknetwork.com
  hsts: false
  https: true
  note: Apex redirects (301) to host.blinknetwork.com. Negotiates only TLSv1.2 - the weakest TLS of any Blink host probed.
  server: awselb/2.0
  tls_version: TLSv1.2
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: host.blinknetwork.eu
  hsts: false
  https: true
  note: European host portal. Returns 403 on /ocpi/cpo/versions.
  server: AmazonS3
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blink Charging Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blink Charging, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blink Charging
provider_slug: blink-charging
slug: blink-charging-domain-security
source_filename: blink-charging-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  0-working/probe-domain-security.py for blinkcharging.com, extended 2026-07-27 with manual\n  openssl/dig/curl probes of the blinknetwork.com API + portal hosts, which the script cannot\n  reach from apis.yml (no baseURL is recorded for this provider).\nhosts:\n- host: blinkcharging.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 05:04:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.blinknetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 12:51:03 2027 GMT\n  hsts: false\n  server: kong/2.8.1\n  note: Public Kong API gateway. No Strict-Transport-Security header on any response.\n- host: host.blinknetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 12:51:03 2027 GMT\n  hsts: false\n  server: AmazonS3\n  note: Blink Network host portal (React SPA on S3/CloudFront). No HSTS.\n- host: blinknetwork.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires:\
  \ Feb 13 12:51:03 2027 GMT\n  hsts: false\n  server: awselb/2.0\n  note: >-\n    Apex redirects (301) to host.blinknetwork.com. Negotiates only TLSv1.2 - the weakest TLS of\n    any Blink host probed.\n- host: host.blinknetwork.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n  server: AmazonS3\n  note: European host portal. Returns 403 on /ocpi/cpo/versions.\ndomains:\n- domain: blinkcharging.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: blinknetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 a mx include:spf.protection.outlook.com include:mail.zendesk.com a:blinknetwork.com\n    a:smtp.blinknetwork.com a:dmz.blinknetwork.com ip4:206.225.165.104 ip4:72.44.248.138\n    include:amazonses.com +all\n  spf_all: +all\n  spf_weakness: >-\n    The SPF record ends in `+all`, which explicitly passes every sender and so neutralises SPF for\n    blinknetwork.com\
  \ - the domain carrying the API gateway and both host portals.\n  dmarc: false\n  dmarc_policy: null\nfindings:\n- No CAA record on either registrable domain - any CA may issue for them.\n- No DNSSEC on either registrable domain.\n- No DMARC record on blinknetwork.com (blinkcharging.com has DMARC at p=quarantine).\n- 'SPF on blinknetwork.com ends in +all: a permissive record that authorises all senders.'\n- HSTS is present on blinkcharging.com only; no blinknetwork.com host sets it.\n- No security.txt on any host (see well-known/blink-charging-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blink-charging/refs/heads/main/security/blink-charging-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- EV Charging
- Electric Vehicles
- Charging Stations
- Grid
- Demand Response
- Fleet Management
- OCPP
- OpenADR
- Roaming
---
