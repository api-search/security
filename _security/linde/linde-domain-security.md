---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linde.com
  spf: true
hosts:
- cert_expires: Oct  7 08:19:32 2026 GMT
  host: www.linde.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.linde.com
  https: false
- cert_expires: Sep 21 09:57:07 2026 GMT
  host: api.linde.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linde Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linde, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Linde
provider_slug: linde
slug: linde-domain-security
source_filename: linde-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.linde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.linde.com\n  https: false\n- host: api.linde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:57:07 2026 GMT\n  hsts: null\ndomains:\n- domain: linde.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linde/refs/heads/main/security/linde-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial Gases
- Engineering
- Chemistry
---
