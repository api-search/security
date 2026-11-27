---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lemmapark.com
  spf: false
hosts:
- cert_expires: Jan 10 18:50:08 2027 GMT
  host: lemmapark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lemma Park Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemma Park, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lemma Park
provider_slug: lemmapark-com
slug: lemmapark-com-domain-security
source_filename: lemmapark-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemmapark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 18:50:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lemmapark.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lemmapark-com/security/lemmapark-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Research Lab
- Mathematics
- AI Agents
- Open Problems
---
