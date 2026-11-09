---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zephior.com
  spf: true
hosts:
- cert_expires: Dec 31 00:58:05 2026 GMT
  host: zephior.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zephior Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zephior-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: zephior-com
provider_slug: zephior-com
slug: zephior-com-domain-security
source_filename: zephior-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zephior.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 00:58:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zephior.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/zephior-com/security/zephior-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Procurement
- Tender
- Marketplace
---
