---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecologi.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: ecologi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 11:24:49 2026 GMT
  host: docs.ecologi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: public.ecologi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecologi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ecologi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ecologi
provider_slug: ecologi
slug: ecologi-domain-security
source_filename: ecologi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecologi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ecologi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 11:24:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public.ecologi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ecologi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecologi/refs/heads/main/security/ecologi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Climate
- Climate Action
- Carbon Offsets
- Carbon Removal
- Carbon Avoidance
- Reforestation
- Tree Planting
- Habitat Restoration
- Sustainability
- ESG
- Net Zero
- B Corp
- Impact
- Verified Carbon
- Reporting
- Zapier
- Shopify
- Webhooks
---
