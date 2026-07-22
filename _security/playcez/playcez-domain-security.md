---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: playcez.com
  spf: true
hosts:
- cert_expires: Sep 18 12:57:22 2026 GMT
  host: playcez.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playcez Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playcez, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Playcez
provider_slug: playcez
slug: playcez-domain-security
source_filename: playcez-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playcez.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 12:57:22 2026 GMT\n  hsts: null\ndomains:\n- domain: playcez.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playcez/refs/heads/main/security/playcez-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
