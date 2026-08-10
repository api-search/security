---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wellthapp.com
  spf: true
hosts:
- cert_expires: Sep 20 17:41:21 2026 GMT
  host: www.wellthapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 11:55:08 2026 GMT
  host: api.wellthapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wellth, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wellth
provider_slug: wellth
slug: wellth-domain-security
source_filename: wellth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wellthapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:41:21 2026 GMT\n  hsts: false\n- host: api.wellthapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 11:55:08 2026 GMT\n  hsts: false\ndomains:\n- domain: wellthapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellth/refs/heads/main/security/wellth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Medication Adherence
- Behavioral Health
- Health Plans
- Medicare
- Medicaid
- Patient Engagement
- Rewards
- GraphQL
- Mobile
---
