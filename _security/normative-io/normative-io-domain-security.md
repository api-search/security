---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: normative.io
  spf: true
hosts:
- cert_expires: Sep 27 10:17:04 2026 GMT
  host: normative.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Normative Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Normative, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Normative
provider_slug: normative-io
slug: normative-io-domain-security
source_filename: normative-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: normative.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:17:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: normative.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/normative-io/refs/heads/main/security/normative-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Carbon Accounting
- ESG Reporting
- Sustainability
- CSRD
- CBAM
- SBTi
- GHG Protocol
- Scope 3 Emissions
- Product Carbon Footprint
- Supply Chain
- Climate Tech
- Net Zero
- Enterprise SaaS
---
