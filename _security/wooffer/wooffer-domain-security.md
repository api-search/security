---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wooffer.io
  spf: true
hosts:
- cert_expires: Dec 17 08:19:01 2026 GMT
  host: wooffer.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wooffer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wooffer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: wooffer
provider_slug: wooffer
slug: wooffer-domain-security
source_filename: wooffer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wooffer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 08:19:01 2026 GMT\n  hsts: false\ndomains:\n- domain: wooffer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/wooffer/security/wooffer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Monitoring
- Server
- Real-time
- SaaS
- Performance
---
