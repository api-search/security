---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "digicert.com"
  - 0 issue "awstrust.com"
  - 128 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sherwin-williams.com
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.sherwin-williams.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: suppliers.sherwin-williams.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sherwin Williams Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sherwin-Williams, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sherwin-Williams
provider_slug: sherwin-williams
slug: sherwin-williams-domain-security
source_filename: sherwin-williams-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sherwin-williams.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: suppliers.sherwin-williams.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: sherwin-williams.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"digicert.com\"\n  - 0 issue \"awstrust.com\"\n  - 128 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sherwin-williams/refs/heads/main/security/sherwin-williams-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Construction
- Fortune 500
- Paints
- Retail
- Supply Chain
---
