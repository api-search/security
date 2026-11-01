---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: takeargmax.com
  spf: true
hosts:
- cert_expires: Dec  4 08:13:38 2026 GMT
  host: www.takeargmax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Takeargmax Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argmax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Argmax
provider_slug: takeargmax-com
slug: takeargmax-com-domain-security
source_filename: takeargmax-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.takeargmax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 08:13:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: takeargmax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/takeargmax-com/security/takeargmax-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Speech
- LanguageModels
- CloudAPI
---
