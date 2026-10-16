---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: seeedstudio.com
  spf: true
hosts:
- cert_expires: Dec 19 08:51:18 2026 GMT
  host: www.seeedstudio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seeed Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seeed Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Seeed Studio
provider_slug: seeed-studio
slug: seeed-studio-domain-security
source_filename: seeed-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seeedstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 08:51:18 2026 GMT\n  hsts: false\ndomains:\n- domain: seeedstudio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seeed-studio/refs/heads/main/security/seeed-studio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- IoT
- Hardware
- OpenSource
- Community
---
