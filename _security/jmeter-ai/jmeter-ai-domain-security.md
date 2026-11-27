---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: jmeter.ai
  spf: false
hosts:
- cert_expires: Dec 14 21:24:07 2026 GMT
  host: jmeter.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JMeter.AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JMeter.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: JMeter.AI
provider_slug: jmeter-ai
slug: jmeter-ai-domain-security
source_filename: jmeter-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jmeter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 21:24:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jmeter.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jmeter-ai/security/jmeter-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Performance
- Artificial Intelligence
- Apache-JMeter
- Plugins
- Automation
---
