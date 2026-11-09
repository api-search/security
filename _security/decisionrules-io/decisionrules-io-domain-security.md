---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: decisionrules.io
  spf: true
hosts:
- cert_expires: Dec  7 02:35:35 2026 GMT
  host: decisionrules.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Decisionrules Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DecisionRules, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DecisionRules
provider_slug: decisionrules-io
slug: decisionrules-io-domain-security
source_filename: decisionrules-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decisionrules.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 02:35:35 2026 GMT\n  hsts: false\ndomains:\n- domain: decisionrules.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/decisionrules-io/security/decisionrules-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Business Rules
- Artificial Intelligence
- Enterprise
- Integration
- Low-Code
---
