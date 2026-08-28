---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neurelis.com
  spf: true
hosts:
- cert_expires: Nov  3 19:08:48 2026 GMT
  host: www.neurelis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neurelis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neurelis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neurelis
provider_slug: neurelis
slug: neurelis-domain-security
source_filename: neurelis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neurelis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 19:08:48 2026 GMT\n  hsts: false\ndomains:\n- domain: neurelis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurelis/refs/heads/main/security/neurelis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Life Sciences
- Healthcare
- Neuroscience
- Epilepsy
- Drug Delivery
- Specialty Pharma
- Biotechnology
---
