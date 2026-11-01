---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thecloudconnectors.com
  spf: true
hosts:
- cert_expires: Dec 31 19:14:10 2026 GMT
  host: thecloudconnectors.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thecloudconnectors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tavio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tavio
provider_slug: thecloudconnectors
slug: thecloudconnectors-domain-security
source_filename: thecloudconnectors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thecloudconnectors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 19:14:10 2026 GMT\n  hsts: null\ndomains:\n- domain: thecloudconnectors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/thecloudconnectors/security/thecloudconnectors-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Integration
- Human Resources
- Supply Chain
- iPaaS
- Automation
---
