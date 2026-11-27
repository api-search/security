---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: garminmcp.com
  spf: true
hosts:
- cert_expires: Dec 16 08:16:07 2026 GMT
  host: garminmcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Garmin MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Garmin MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Garmin MCP
provider_slug: garminmcp-com
slug: garminmcp-com-domain-security
source_filename: garminmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: garminmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 08:16:07 2026 GMT\n  hsts: false\ndomains:\n- domain: garminmcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/garminmcp-com/security/garminmcp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Wearables
- AI Integration
- Fitness
- Data Connector
---
