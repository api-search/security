---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usetyton.com
  spf: true
hosts:
- cert_expires: Dec 25 00:17:46 2026 GMT
  host: usetyton.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usetyton Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for usetyton-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: usetyton-com
provider_slug: usetyton-com
slug: usetyton-com-domain-security
source_filename: usetyton-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usetyton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 00:17:46 2026 GMT\n  hsts: false\ndomains:\n- domain: usetyton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/usetyton-com/security/usetyton-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Meta Pixel
- Conversions API
- Marketing
- Automation
---
