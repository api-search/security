---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nearius.com
  spf: true
hosts:
- cert_expires: Jan 28 10:33:05 2027 GMT
  host: nearius.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nearius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nearius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nearius
provider_slug: nearius-com
slug: nearius-com-domain-security
source_filename: nearius-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nearius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 10:33:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nearius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nearius-com/security/nearius-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Legal Tech
- Jurisprudence
- LLM
---
