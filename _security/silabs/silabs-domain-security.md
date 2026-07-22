---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "thawte.com"
  - 0 iodef "mailto:noc@silabs.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: silabs.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: silabs.com
  hsts: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silicon Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Silicon Labs
provider_slug: silabs
slug: silabs-domain-security
source_filename: silabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\ndomains:\n- domain: silabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"thawte.com\"\n  - 0 iodef \"mailto:noc@silabs.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silabs/refs/heads/main/security/silabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Internet of Things
- Wireless
- Microcontrollers
- Bluetooth
- Zigbee
- Matter
- Embedded
- Developer Tools
---
