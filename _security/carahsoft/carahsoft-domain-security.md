---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carahsoft.com
  spf: true
hosts:
- cert_expires: Oct 20 16:24:59 2026 GMT
  host: www.carahsoft.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 16:24:59 2026 GMT
  host: developer.carahsoft.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carahsoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carahsoft, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carahsoft
provider_slug: carahsoft
slug: carahsoft-domain-security
source_filename: carahsoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carahsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 16:24:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.carahsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 16:24:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carahsoft.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carahsoft/refs/heads/main/security/carahsoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government IT
- Public Sector
- Reseller
- Distributor
- Procurement
- Contract Vehicles
- Federal
- State and Local
---
