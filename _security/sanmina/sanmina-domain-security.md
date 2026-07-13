---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sanmina.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 42-q.com
  spf: true
hosts:
- cert_expires: Oct  6 03:45:45 2026 GMT
  host: www.sanmina.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 03:46:35 2026 GMT
  host: www.42-q.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sanmina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sanmina, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sanmina
provider_slug: sanmina
slug: sanmina-domain-security
source_filename: sanmina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sanmina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.42-q.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:46:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sanmina.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 42-q.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanmina/refs/heads/main/security/sanmina-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- Contract Manufacturing
- MES
- Supply Chain
- Industrial
- Enterprise
- Fortune 500
---
