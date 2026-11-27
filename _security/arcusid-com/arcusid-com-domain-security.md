---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arcusid.com
  spf: false
hosts:
- cert_expires: Dec 26 19:16:44 2026 GMT
  host: arcusid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ArcID Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ArcID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ArcID
provider_slug: arcusid-com
slug: arcusid-com-domain-security
source_filename: arcusid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcusid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 19:16:44 2026 GMT\n  hsts: false\ndomains:\n- domain: arcusid.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/arcusid-com/security/arcusid-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Identity
- Artificial Intelligence
- Blockchain
- Arc
- ERC-8004
- USDC
---
