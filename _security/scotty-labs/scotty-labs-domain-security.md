---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: scotty.ai
  spf: false
hosts:
- cert_expires: Dec 13 00:32:50 2026 GMT
  host: www.scotty.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scotty Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scotty Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Scotty Labs
provider_slug: scotty-labs
slug: scotty-labs-domain-security
source_filename: scotty-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scotty.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 00:32:50 2026 GMT\n  hsts: false\ndomains:\n- domain: scotty.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/scotty-labs/security/scotty-labs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
---
