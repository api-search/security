---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lnw.com
  spf: true
hosts:
- cert_expires: Aug 13 05:15:28 2026 GMT
  host: www.lnw.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 09:16:38 2027 GMT
  host: portal.lnw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Light And Wonder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Light & Wonder, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Light & Wonder
provider_slug: light-and-wonder
slug: light-and-wonder-domain-security
source_filename: light-and-wonder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lnw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 05:15:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.lnw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 09:16:38 2027 GMT\n  hsts: false\ndomains:\n- domain: lnw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/light-and-wonder/refs/heads/main/security/light-and-wonder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Casino
- iGaming
- Mobile Games
- Entertainment
---
