---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prodpoke.com
  spf: true
hosts:
- cert_expires: Dec 19 20:39:34 2026 GMT
  host: prodpoke.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prodpoke Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for prodpoke-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: prodpoke-com
provider_slug: prodpoke-com
slug: prodpoke-com-domain-security
source_filename: prodpoke-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prodpoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 20:39:34 2026 GMT\n  hsts: false\ndomains:\n- domain: prodpoke.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/prodpoke-com/security/prodpoke-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Testing
- Automation
- QA
- Developer Tools
- Web
---
