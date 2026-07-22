---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: praxair.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lindeus.com
  spf: true
hosts:
- cert_expires: Oct  7 08:19:32 2026 GMT
  host: www.praxair.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 08:19:32 2026 GMT
  host: www.lindeus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Praxair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Praxair, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Praxair
provider_slug: praxair
slug: praxair-domain-security
source_filename: praxair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.praxair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.lindeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: praxair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lindeus.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/praxair/refs/heads/main/security/praxair-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial Gases
- Manufacturing
- Energy
- Chemicals
- Fortune 500
---
