---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: validis.com
  spf: true
hosts:
- cert_expires: Nov 30 02:50:07 2026 GMT
  host: validis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Validis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Validis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Validis
provider_slug: validis
slug: validis-domain-security
source_filename: validis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: validis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 02:50:07 2026 GMT\n  hsts: false\ndomains:\n- domain: validis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/validis/security/validis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Audit
- Commercial Lending
- Specialist Lending
- M&A Due Diligence
- Financial Data Infrastructure
- API
---
