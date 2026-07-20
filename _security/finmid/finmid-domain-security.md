---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finmid.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.finmid.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:14:42 2026 GMT
  host: docs.finmid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.finmid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finmid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finmid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Finmid
provider_slug: finmid
slug: finmid-domain-security
source_filename: finmid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finmid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: docs.finmid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:14:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.finmid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: finmid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/security/finmid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Embedded Finance
- Embedded Lending
- B2B Payments
- Fintech
- Lending
- Capital
- Financing
- Payments
- Marketplaces
---
