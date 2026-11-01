---
description: ''
domains:
- caa:
  - dlnnvtnsdry8x.cloudfront.net.
  dmarc: false
  dnssec: true
  domain: junct.dev
  spf: true
hosts:
- cert_expires: Apr 23 23:59:59 2027 GMT
  host: junct.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Junct Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for junct-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: junct-dev
provider_slug: junct-dev
slug: junct-dev-domain-security
source_filename: junct-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: junct.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: junct.dev\n  dnssec: true\n  caa:\n  - dlnnvtnsdry8x.cloudfront.net.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/junct-dev/security/junct-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- AI
- Agent
- MCP
- API Tools
- Platform
---
