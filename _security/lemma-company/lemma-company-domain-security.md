---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: lemma.company
  spf: true
hosts:
- cert_expires: Feb 13 06:08:53 2027 GMT
  host: lemma.company
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lemma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Lemma
provider_slug: lemma-company
slug: lemma-company-domain-security
source_filename: lemma-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemma.company\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 06:08:53 2027 GMT\n  hsts: false\ndomains:\n- domain: lemma.company\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lemma-company/security/lemma-company-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Artificial Intelligence
- Agents
- Design
- Studio
- Telegram
---
