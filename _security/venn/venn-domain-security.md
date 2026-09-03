---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: venn.city
  spf: true
hosts:
- cert_expires: Oct 10 13:16:22 2026 GMT
  host: venn.city
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: docs.venn.city
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.venn.city
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Venn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Venn, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Venn
provider_slug: venn
slug: venn-domain-security
source_filename: venn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: venn.city\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 13:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.venn.city\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: false\n- host: api.venn.city\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: venn.city\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venn/refs/heads/main/security/venn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Management
- Multifamily
- Resident Experience
- Proptech
- Leasing
- Community
- Payments
- GraphQL
- Mobile Apps
---
