---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: astra3.com
  spf: true
hosts:
- cert_expires: Oct  2 19:47:19 2026 GMT
  host: astra3.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Astra3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astra3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Astra3
provider_slug: astra3
slug: astra3-domain-security
source_filename: astra3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astra3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:47:19 2026 GMT\n  hsts: false\ndomains:\n- domain: astra3.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astra3/refs/heads/main/security/astra3-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Technology
- Finance
- Data
- Services
---
