---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: silicondust.com
  spf: true
hosts:
- cert_expires: Jan 15 22:18:18 2027 GMT
  host: silicondust.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Silicondust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SiliconDust (HDHomeRun), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SiliconDust (HDHomeRun)
provider_slug: silicondust
slug: silicondust-domain-security
source_filename: silicondust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silicondust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 22:18:18 2027 GMT\n  hsts: false\ndomains:\n- domain: silicondust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/silicondust/security/silicondust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hardware
- Streaming
- TV
- Consumer Electronics
---
