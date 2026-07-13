---
api_specs:
- filename: clickfunnels-openapi.yml
  format: yaml
  label: ClickFunnels 2.0 API
  slug: clickfunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/openapi/clickfunnels-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clickfunnels.com
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myclickfunnels.com
  spf: true
hosts:
- cert_expires: Sep  4 08:17:59 2026 GMT
  host: www.clickfunnels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 06:51:37 2026 GMT
  host: developers.myclickfunnels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 01:15:07 2026 GMT
  host: accounts.myclickfunnels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clickfunnels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClickFunnels, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClickFunnels
provider_slug: clickfunnels
slug: clickfunnels-domain-security
source_filename: clickfunnels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clickfunnels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 08:17:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.myclickfunnels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:51:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: accounts.myclickfunnels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:15:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clickfunnels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: myclickfunnels.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/security/clickfunnels-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Funnels
- Landing Pages
- E-commerce
- Marketing
- Checkout
- CRM
---
