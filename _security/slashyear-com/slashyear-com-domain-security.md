---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: slashyear.com
  spf: true
hosts:
- cert_expires: Dec  5 17:07:08 2026 GMT
  host: slashyear.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Slashyear Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SlashYear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SlashYear
provider_slug: slashyear-com
slug: slashyear-com-domain-security
source_filename: slashyear-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slashyear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 17:07:08 2026 GMT\n  hsts: false\ndomains:\n- domain: slashyear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/slashyear-com/security/slashyear-com-domain-security.yml
summary_line: TLSv1.3
tags:
- History
- Data
- API
- Open
- Free
---
