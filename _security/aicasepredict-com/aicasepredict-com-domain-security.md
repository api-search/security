---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ai-cases.com
  spf: true
hosts:
- cert_expires: Jan 19 06:26:51 2027 GMT
  host: ai-cases.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Cases Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Cases, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Cases
provider_slug: aicasepredict-com
slug: aicasepredict-com-domain-security
source_filename: aicasepredict-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-cases.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 06:26:51 2027 GMT\n  hsts: false\ndomains:\n- domain: ai-cases.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aicasepredict-com/security/aicasepredict-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Platform
- Predictive Analytics
- Use Cases
- Industry Solutions
---
