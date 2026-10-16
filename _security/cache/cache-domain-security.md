---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usecache.com
  spf: true
hosts:
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: usecache.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cache Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cache, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cache
provider_slug: cache
slug: cache-domain-security
source_filename: cache-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usecache.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usecache.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cache/refs/heads/main/security/cache-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Finance
- Investment
- Tax-Optimization
- Wealth-Management
- Platform
---
