---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: discolike.com
  spf: true
hosts:
- cert_expires: Dec 10 00:24:14 2026 GMT
  host: discolike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DiscoLike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DiscoLike, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DiscoLike
provider_slug: discolike-com
slug: discolike-com-domain-security
source_filename: discolike-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: discolike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 00:24:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: discolike.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/discolike-com/security/discolike-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Market Intelligence
- Data Aggregation
- API Platform
- Competitive Analysis
---
