---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: caliper.fit
  spf: true
hosts:
- cert_expires: Dec 21 17:02:07 2026 GMT
  host: caliper.fit
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caliper Fit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for caliper-fit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: caliper-fit
provider_slug: caliper-fit
slug: caliper-fit-domain-security
source_filename: caliper-fit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caliper.fit\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 17:02:07 2026 GMT\n  hsts: null\ndomains:\n- domain: caliper.fit\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/caliper-fit/security/caliper-fit-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Geometry
- CAD
- Metadata
- API
- MCP
---
