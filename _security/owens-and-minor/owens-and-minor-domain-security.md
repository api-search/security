---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:seceng.seceng@owens-minor.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: owens-minor.com
  spf: true
hosts:
- cert_expires: Sep 26 08:03:44 2026 GMT
  host: www.owens-minor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Owens And Minor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Owens & Minor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Owens & Minor
provider_slug: owens-and-minor
slug: owens-and-minor-domain-security
source_filename: owens-and-minor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.owens-minor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:03:44 2026 GMT\n  hsts: false\ndomains:\n- domain: owens-minor.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:seceng.seceng@owens-minor.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owens-and-minor/refs/heads/main/security/owens-and-minor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 500
- Healthcare
- Medical Supplies
- Distribution
- Logistics
---
