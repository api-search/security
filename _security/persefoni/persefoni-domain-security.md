---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: persefoni.com
  spf: true
hosts:
- cert_expires: Aug 16 16:50:17 2026 GMT
  host: www.persefoni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Persefoni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Persefoni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Persefoni
provider_slug: persefoni
slug: persefoni-domain-security
source_filename: persefoni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.persefoni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:50:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: persefoni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persefoni/refs/heads/main/security/persefoni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Climate
- Carbon Accounting
- CMAP
- ESG
- Financed Emissions
- PCAF
- Disclosure
- CSRD
- SBTi
- Sustainability
- Enterprise
---
