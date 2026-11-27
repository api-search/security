---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: sunaivacore.io
  spf: true
hosts:
- cert_expires: Jan  3 11:03:51 2027 GMT
  host: sunaivacore.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sunaiva Core Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunaiva Core, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sunaiva Core
provider_slug: sunaivacore-io
slug: sunaivacore-io-domain-security
source_filename: sunaivacore-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunaivacore.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 11:03:51 2027 GMT\n  hsts: false\ndomains:\n- domain: sunaivacore.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/sunaivacore-io/security/sunaivacore-io-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Validation
- MCP-native
- Compliance
- Audit
---
