---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: aqemia.com
  spf: true
hosts:
- cert_expires: Nov 10 05:53:48 2026 GMT
  host: aqemia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aqemia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AQEMIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: AQEMIA
provider_slug: aqemia
slug: aqemia-domain-security
source_filename: aqemia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aqemia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 05:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aqemia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqemia/refs/heads/main/security/aqemia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- AI
- DrugDiscovery
- Biotechnology
- Platform
---
