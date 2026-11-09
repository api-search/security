---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: beyondfolder.com
  spf: true
hosts:
- cert_expires: Dec  6 22:49:14 2026 GMT
  host: beyondfolder.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beyondfolder Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeyondFolder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BeyondFolder
provider_slug: beyondfolder-com
slug: beyondfolder-com-domain-security
source_filename: beyondfolder-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beyondfolder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 22:49:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: beyondfolder.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/beyondfolder-com/security/beyondfolder-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software
- Tools
- Email
- DMARC
- Calculators
---
