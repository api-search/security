---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gao.gov
  spf: true
hosts:
- cert_expires: Oct 25 12:20:11 2026 GMT
  host: www.gao.gov
  hsts: true
  hsts_max_age: 15768000
  hsts_note: 'Corrected by hand 2026-09-12. The automated probe recorded null because www.gao.gov''s Akamai Bot Manager answers a plain HEAD with 403; the 403 response itself still carries strict-transport-security: max-age=15768000, confirmed with a browser header set.'
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Government Accountability Office Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Government Accountability Office, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Government Accountability Office
provider_slug: government-accountability-office
slug: government-accountability-office-domain-security
source_filename: government-accountability-office-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gao.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 12:20:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_note: >-\n    Corrected by hand 2026-09-12. The automated probe recorded null because www.gao.gov's\n    Akamai Bot Manager answers a plain HEAD with 403; the 403 response itself still carries\n    strict-transport-security: max-age=15768000, confirmed with a browser header set.\ndomains:\n- domain: gao.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/government-accountability-office/refs/heads/main/security/government-accountability-office-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accountability
- Auditing
- Federal-Government
- Government
- United States
---
