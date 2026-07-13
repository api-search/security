---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astm.org
  spf: true
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: www.astm.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: compass.astm.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: store.astm.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astm International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASTM International, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ASTM International
provider_slug: astm-international
slug: astm-international-domain-security
source_filename: astm-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astm.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: null\n- host: compass.astm.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: store.astm.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: astm.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astm-international/refs/heads/main/security/astm-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Standards
- Standards Development Organization
- Consensus Standards
- Technical Committees
- Materials Testing
- Specifications
- Test Methods
- Certification
- Voluntary Standards
- International
---
