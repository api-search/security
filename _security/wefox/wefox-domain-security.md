---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wefox.com
  spf: true
hosts:
- cert_expires: Oct  8 19:06:06 2026 GMT
  host: www.wefox.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wefox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wefox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: wefox
provider_slug: wefox
slug: wefox-domain-security
source_filename: wefox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wefox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:06:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: wefox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wefox/refs/heads/main/security/wefox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Digital Insurance
- Insurance Distribution
- Broker Platform
- Motor Insurance
- Home Insurance
- Liability Insurance
- Life Insurance
- Commercial Insurance
- Europe
- Germany
- Berlin
- Financial Services
---
