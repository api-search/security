---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aicodelabs.dev
  spf: false
hosts:
- cert_expires: Dec 10 20:04:10 2026 GMT
  host: aicodelabs.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Code Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Code Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AI Code Labs
provider_slug: aicodelabs-dev
slug: aicodelabs-dev-domain-security
source_filename: aicodelabs-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aicodelabs.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 20:04:10 2026 GMT\n  hsts: false\ndomains:\n- domain: aicodelabs.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aicodelabs-dev/security/aicodelabs-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- .NET
- Code Modernization
- Experiments
---
