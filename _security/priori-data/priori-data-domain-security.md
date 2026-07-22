---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prioridata.com
  spf: true
hosts:
- cert_expires: Aug 25 17:33:32 2026 GMT
  host: prioridata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Priori Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Priori Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Priori Data
provider_slug: priori-data
slug: priori-data-domain-security
source_filename: priori-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prioridata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:33:32 2026 GMT\n  hsts: false\ndomains:\n- domain: prioridata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/priori-data/refs/heads/main/security/priori-data-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
