---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hemlane.com
  spf: true
hosts:
- cert_expires: Aug 15 01:27:44 2026 GMT
  host: www.hemlane.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hemlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hemlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hemlane
provider_slug: hemlane
slug: hemlane-domain-security
source_filename: hemlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hemlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 01:27:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hemlane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hemlane/refs/heads/main/security/hemlane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Property Management
- Real Estate
- Rental
- Tenant Screening
- Lease Management
- Rent Collection
- Maintenance
- Landlord
---
