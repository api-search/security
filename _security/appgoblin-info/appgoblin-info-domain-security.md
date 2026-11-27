---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appgoblin.info
  spf: true
hosts:
- cert_expires: Dec 12 05:59:14 2026 GMT
  host: appgoblin.info
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AppGoblin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppGoblin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppGoblin
provider_slug: appgoblin-info
slug: appgoblin-info-domain-security
source_filename: appgoblin-info-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appgoblin.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 05:59:14 2026 GMT\n  hsts: false\ndomains:\n- domain: appgoblin.info\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/appgoblin-info/security/appgoblin-info-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Mobile
- Marketing
- Analytics
- B2B
- Intelligence
---
