---
description: ''
domains:
- caa:
  - 0 iodef "mailto:hello@elevai.ch"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: elevai.ch
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: elevai.ch
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: elevai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for elevai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: elevai
provider_slug: elevai-ch
slug: elevai-ch-domain-security
source_filename: elevai-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elevai.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: elevai.ch\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:hello@elevai.ch\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/elevai-ch/security/elevai-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Lab
- Switzerland
- Machine Learning
- Innovation
---
