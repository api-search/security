---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sophontai.com
  spf: true
hosts:
- cert_expires: Dec  7 19:37:37 2026 GMT
  host: sophontai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sophontai Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sophontai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sophontai
provider_slug: sophontai-com
slug: sophontai-com-domain-security
source_filename: sophontai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sophontai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 19:37:37 2026 GMT\n  hsts: false\ndomains:\n- domain: sophontai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/sophontai-com/security/sophontai-com-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Medical
- Healthcare
- OpenSource
- Superintelligence
---
