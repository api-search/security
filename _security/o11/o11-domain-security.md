---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: o11.ai
  spf: true
hosts:
- cert_expires: Oct 10 15:56:25 2026 GMT
  host: o11.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: O11 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for O11, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: O11
provider_slug: o11
slug: o11-domain-security
source_filename: o11-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: o11.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 15:56:25 2026 GMT\n  hsts: false\ndomains:\n- domain: o11.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/o11/refs/heads/main/security/o11-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Financial Services
- Fintech
- Workflow Automation
- Enterprise Software
- Document Generation
- Y Combinator
---
