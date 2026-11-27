---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowaiapi.com
  spf: true
hosts:
- cert_expires: Jan 11 18:10:39 2027 GMT
  host: flowaiapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flow AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flow AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flow AI
provider_slug: flowaiapi-com
slug: flowaiapi-com-domain-security
source_filename: flowaiapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowaiapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 18:10:39 2027 GMT\n  hsts: false\ndomains:\n- domain: flowaiapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/flowaiapi-com/security/flowaiapi-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Inference
- Managed
- OpenAI
- Anthropic
---
