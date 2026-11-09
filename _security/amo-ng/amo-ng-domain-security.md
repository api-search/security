---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amo.ng
  spf: true
hosts:
- cert_expires: Dec 27 15:16:51 2026 GMT
  host: amo.ng
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amo Ng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amo.ng, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amo.ng
provider_slug: amo-ng
slug: amo-ng-domain-security
source_filename: amo-ng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amo.ng\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 15:16:51 2026 GMT\n  hsts: false\ndomains:\n- domain: amo.ng\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/amo-ng/security/amo-ng-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Prompts
- Workflows
- Skills
- Productivity
---
