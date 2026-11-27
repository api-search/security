---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: alpnai.com
  spf: false
hosts:
- cert_expires: Dec 13 00:17:41 2026 GMT
  host: alpnai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ALPNAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ALPNAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: ALPNAI
provider_slug: alpnai-com
slug: alpnai-com-domain-security
source_filename: alpnai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alpnai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 00:17:41 2026 GMT\n  hsts: false\ndomains:\n- domain: alpnai.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/alpnai-com/security/alpnai-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Artificial Intelligence
- Software-as-a-Service
- Performance
- Analytics
- Swiss
---
