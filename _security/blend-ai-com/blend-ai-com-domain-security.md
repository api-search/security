---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blend-ai.com
  spf: true
hosts:
- cert_expires: Jan 24 21:10:57 2027 GMT
  host: blend-ai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blend AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blend AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blend AI
provider_slug: blend-ai-com
slug: blend-ai-com-domain-security
source_filename: blend-ai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blend-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 21:10:57 2027 GMT\n  hsts: false\ndomains:\n- domain: blend-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/blend-ai-com/security/blend-ai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Artificial Intelligence
- Marketing
- Automation
---
