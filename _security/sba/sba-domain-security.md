---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sba.gov
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.sba.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: developer.sba.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.sba.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Small Business Administration (SBA), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Small Business Administration (SBA)
provider_slug: sba
slug: sba-domain-security
source_filename: sba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sba.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sba.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sba.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sba.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sba/refs/heads/main/security/sba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Small Business
- Loans
- Certifications
- Contracting
- Disaster Assistance
- SBIR
- STTR
---
