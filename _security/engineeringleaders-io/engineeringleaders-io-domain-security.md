---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: engineeringleaders.io
  spf: true
hosts:
- cert_expires: Jan 20 16:14:14 2027 GMT
  host: engineeringleaders.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Engineeringleaders Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for engineeringleaders-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: engineeringleaders-io
provider_slug: engineeringleaders-io
slug: engineeringleaders-io-domain-security
source_filename: engineeringleaders-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: engineeringleaders.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 16:14:14 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: engineeringleaders.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/engineeringleaders-io/security/engineeringleaders-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Community
- Leadership
- Events
- Membership
---
