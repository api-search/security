---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wevorce.com
  spf: true
hosts:
- cert_expires: Sep 27 09:02:03 2026 GMT
  host: wevorce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wevorce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wevorce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wevorce
provider_slug: wevorce
slug: wevorce-domain-security
source_filename: wevorce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wevorce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:02:03 2026 GMT\n  hsts: null\ndomains:\n- domain: wevorce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wevorce/refs/heads/main/security/wevorce-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Legal
- Legal Tech
- Divorce
- Family Law
- Mediation
---
