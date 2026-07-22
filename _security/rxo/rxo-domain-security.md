---
description: ''
domains:
- caa:
  - 0 iodef "mailto:hostmaster@rxo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "ssl.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rxo.com
  spf: true
hosts:
- cert_expires: Sep  9 03:59:11 2026 GMT
  host: www.rxo.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rxo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RXO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RXO
provider_slug: rxo
slug: rxo-domain-security
source_filename: rxo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rxo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:59:11 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: rxo.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hostmaster@rxo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rxo/refs/heads/main/security/rxo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Transportation
- Freight
- Supply Chain
- Trucking
---
