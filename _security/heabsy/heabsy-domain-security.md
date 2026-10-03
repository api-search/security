---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heabsy.com
  spf: true
hosts:
- cert_expires: Dec 19 18:57:12 2026 GMT
  host: heabsy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heabsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heabsy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Heabsy
provider_slug: heabsy
slug: heabsy-domain-security
source_filename: heabsy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heabsy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 18:57:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heabsy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heabsy/refs/heads/main/security/heabsy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Inference
- OpenAI-Compatible
- EU-regulated
- Software-as-a-Service
---
