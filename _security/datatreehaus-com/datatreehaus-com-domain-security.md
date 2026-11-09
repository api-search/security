---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datatreehaus.com
  spf: true
hosts:
- cert_expires: Dec 10 09:31:46 2026 GMT
  host: datatreehaus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datatreehaus Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datatreehaus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datatreehaus
provider_slug: datatreehaus-com
slug: datatreehaus-com-domain-security
source_filename: datatreehaus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datatreehaus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 09:31:46 2026 GMT\n  hsts: false\ndomains:\n- domain: datatreehaus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datatreehaus-com/security/datatreehaus-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software Studio
- API-First
- MCP
- United Kingdom
- Web Applications
---
