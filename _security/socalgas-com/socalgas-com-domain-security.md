---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: socalgas.com
  spf: true
hosts:
- cert_expires: Dec 24 21:04:15 2026 GMT
  host: www.socalgas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Socalgas Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Southern California Gas Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Southern California Gas Company
provider_slug: socalgas-com
slug: socalgas-com-domain-security
source_filename: socalgas-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.socalgas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 21:04:15 2026 GMT\n  hsts: null\ndomains:\n- domain: socalgas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socalgas-com/refs/heads/main/security/socalgas-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Utilities
- Natural Gas
---
