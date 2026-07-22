---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meqsolutions.com
  spf: false
hosts:
- cert_expires: Sep  6 06:06:20 2026 GMT
  host: meqsolutions.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meq Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MEQ Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: MEQ Solutions
provider_slug: meq-solutions
slug: meq-solutions-domain-security
source_filename: meq-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meqsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:06:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: meqsolutions.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meq-solutions/refs/heads/main/security/meq-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Agrifood
- Food
- Meat
- Livestock
- Measurement
- Quality Assurance
- Technology
- Hardware
---
