---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clearmind-capital.com
  spf: true
hosts:
- cert_expires: Dec 20 15:00:49 2026 GMT
  host: clearmind-capital.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clearmind Capital Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearMind Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClearMind Capital
provider_slug: clearmind-capital-com
slug: clearmind-capital-com-domain-security
source_filename: clearmind-capital-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearmind-capital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 15:00:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: clearmind-capital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/clearmind-capital-com/security/clearmind-capital-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Financial Planning
- Fiduciary
- Columbus
- Wealth Management
---
