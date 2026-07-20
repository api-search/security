---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: channelengine.com
  spf: true
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: channelengine.net
  spf: true
hosts:
- cert_expires: Sep 18 19:02:30 2026 GMT
  host: www.channelengine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:42:59 2026 GMT
  host: support.channelengine.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:07:41 2026 GMT
  host: demo.channelengine.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Channelengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChannelEngine, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChannelEngine
provider_slug: channelengine
slug: channelengine-domain-security
source_filename: channelengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.channelengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:02:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.channelengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:42:59 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: demo.channelengine.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:07:41 2026 GMT\n  hsts: null\ndomains:\n- domain: channelengine.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: channelengine.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channelengine/refs/heads/main/security/channelengine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Marketplace Integration
- Multichannel Commerce
- Order Management
- Inventory Management
- Product Information
- Retail
- Webhooks
- Netherlands
---
