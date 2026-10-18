---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: buyersight.io
  spf: true
hosts:
- cert_expires: Dec 18 05:33:03 2026 GMT
  host: buyersight.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buyersight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buyersight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Buyersight
provider_slug: buyersight
slug: buyersight-domain-security
source_filename: buyersight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buyersight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 05:33:03 2026 GMT\n  hsts: false\ndomains:\n- domain: buyersight.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buyersight/refs/heads/main/security/buyersight-domain-security.yml
summary_line: TLSv1.3
tags:
- Sales
- Artificial Intelligence
- Outbound
- B2B
- Marketing
---
