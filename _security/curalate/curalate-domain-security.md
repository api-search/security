---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: curalate.com
  spf: true
hosts:
- cert_expires: Jan  5 18:26:21 2027 GMT
  host: www.curalate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curalate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curalate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Curalate
provider_slug: curalate
slug: curalate-domain-security
source_filename: curalate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curalate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 18:26:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curalate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curalate/refs/heads/main/security/curalate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Visual Commerce
- Influencer Marketing
- Social Shopping
- Analytics
- E-Commerce
---
