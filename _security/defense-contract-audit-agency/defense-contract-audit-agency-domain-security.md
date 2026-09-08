---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dcaa.mil
  spf: true
hosts:
- cert_expires: Nov  2 19:35:49 2026 GMT
  host: www.dcaa.mil
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 17:19:12 2026 GMT
  host: fao.dcaa.mil
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 11 17:19:12 2026 GMT
  host: csp.dcaa.mil
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Defense Contract Audit Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Contract Audit Agency, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Contract Audit Agency
provider_slug: defense-contract-audit-agency
slug: defense-contract-audit-agency-domain-security
source_filename: defense-contract-audit-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dcaa.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:35:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fao.dcaa.mil\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 17:19:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: true\n- host: csp.dcaa.mil\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 17:19:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: true\ndomains:\n- domain: dcaa.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnotes:\n- >-\n  HSTS was re-read by hand on 2026-09-07 with a browser User-Agent because the mechanical\n  probe recorded null on all three hosts. All three do send Strict-Transport-Security on\n  GET / : www.dcaa.mil max-age=31536000, fao.dcaa.mil and csp.dcaa.mil\n  max-age=31557600;\
  \ includeSubDomains.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-contract-audit-agency/refs/heads/main/security/defense-contract-audit-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal-Government
- Defense
- Department of Defense
- Audit
- Contract Audit
- Financial
- Government Contracting
- CAGE Code
- Unique Entity Identifier
- Locator
---
