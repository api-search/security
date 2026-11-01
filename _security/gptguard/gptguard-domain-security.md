---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gptguard.ai
  spf: false
hosts:
- cert_expires: Dec 19 20:03:14 2026 GMT
  host: gptguard.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gptguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Protecto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Protecto
provider_slug: gptguard
slug: gptguard-domain-security
source_filename: gptguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gptguard.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 20:03:14 2026 GMT\n  hsts: false\ndomains:\n- domain: gptguard.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gptguard/security/gptguard-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Privacy
- Enterprise
- Fintech
- Data Protection
---
