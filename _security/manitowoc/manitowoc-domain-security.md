---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: manitowoc.com
  spf: true
hosts:
- cert_expires: Sep 25 11:21:12 2026 GMT
  host: www.manitowoc.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manitowoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manitowoc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Manitowoc
provider_slug: manitowoc
slug: manitowoc-domain-security
source_filename: manitowoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.manitowoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:21:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: manitowoc.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manitowoc/refs/heads/main/security/manitowoc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cranes
- Construction
- Lifting Equipment
- Industrial
- Fortune 1000
---
