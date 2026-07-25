---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coastcapitalsavings.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.coastcapitalsavings.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coast Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coast Capital Savings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coast Capital Savings
provider_slug: coast-capital
slug: coast-capital-domain-security
source_filename: coast-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coastcapitalsavings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coastcapitalsavings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coast-capital/refs/heads/main/security/coast-capital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Banking
- Canada
- Credit Union
- Cooperative
- Consumer-Driven Banking
- Data Aggregation
---
