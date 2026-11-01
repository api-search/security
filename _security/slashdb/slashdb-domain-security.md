---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: slashdb.com
  spf: true
hosts:
- cert_expires: Dec  5 22:02:38 2026 GMT
  host: slashdb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Slashdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VT Enterprise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VT Enterprise
provider_slug: slashdb
slug: slashdb-domain-security
source_filename: slashdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slashdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 22:02:38 2026 GMT\n  hsts: false\ndomains:\n- domain: slashdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/slashdb/security/slashdb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API
- Data Integration
- Low Code
- Enterprise Software
- Database APIs
---
