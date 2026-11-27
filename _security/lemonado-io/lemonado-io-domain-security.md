---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lemonado.io
  spf: true
hosts:
- cert_expires: Dec 31 22:41:34 2026 GMT
  host: lemonado.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lemonado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemonado, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lemonado
provider_slug: lemonado-io
slug: lemonado-io-domain-security
source_filename: lemonado-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemonado.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 22:41:34 2026 GMT\n  hsts: false\ndomains:\n- domain: lemonado.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lemonado-io/security/lemonado-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Marketing
- Automation
- Analytics
---
