---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fireflylearning.com
  spf: true
hosts:
- cert_expires: Feb  2 03:43:58 2027 GMT
  host: fireflylearning.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firefly Learning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firefly Learning, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Firefly Learning
provider_slug: firefly-learning
slug: firefly-learning-domain-security
source_filename: firefly-learning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fireflylearning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 03:43:58 2027 GMT\n  hsts: false\ndomains:\n- domain: fireflylearning.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/firefly-learning/security/firefly-learning-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- EdTech
- Software-as-a-Service
- Schools
- Learning
---
