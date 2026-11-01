---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inter-operate.com
  spf: true
hosts:
- cert_expires: Dec 16 01:27:11 2026 GMT
  host: inter-operate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inter Operate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InterOperate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InterOperate
provider_slug: inter-operate
slug: inter-operate-domain-security
source_filename: inter-operate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inter-operate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 01:27:11 2026 GMT\n  hsts: false\ndomains:\n- domain: inter-operate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inter-operate/security/inter-operate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Integration
- Automation
- iPaaS
- Enterprise
- Workflows
---
