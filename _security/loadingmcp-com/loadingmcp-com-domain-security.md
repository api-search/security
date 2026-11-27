---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: loadingmcp.com
  spf: false
hosts:
- cert_expires: Jan 15 22:04:53 2027 GMT
  host: loadingmcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LoadingMCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LoadingMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LoadingMCP
provider_slug: loadingmcp-com
slug: loadingmcp-com-domain-security
source_filename: loadingmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loadingmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 22:04:53 2027 GMT\n  hsts: false\ndomains:\n- domain: loadingmcp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/loadingmcp-com/security/loadingmcp-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Logistics
- 3DPlanning
- ContainerLoading
- Compliance
- Transportation
---
