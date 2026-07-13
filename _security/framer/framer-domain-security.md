---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@framer.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: framer.com
  spf: true
- caa:
  - 0 iodef "mailto:security@framer.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: framerusercontent.com
  spf: false
hosts:
- cert_expires: Sep  7 09:31:09 2026 GMT
  host: www.framer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: framerusercontent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: framer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Framer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Framer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Framer
provider_slug: framer
slug: framer-domain-security
source_filename: framer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.framer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 09:31:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: framerusercontent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: framer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: framer.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@framer.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: framerusercontent.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@framer.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf:\
  \ false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/framer/refs/heads/main/security/framer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Design
- No-Code
- Web Design
- SaaS
---
