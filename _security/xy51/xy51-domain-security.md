---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xy51.com
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: xy51.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xy51 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xiao-Y Technology (小y科技), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Xiao-Y Technology (小y科技)
provider_slug: xy51
slug: xy51-domain-security
source_filename: xy51-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xy51.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: xy51.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xy51/refs/heads/main/security/xy51-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Smart TV
- Entertainment
- Mobile Games
- Game Publishing
- China
---
