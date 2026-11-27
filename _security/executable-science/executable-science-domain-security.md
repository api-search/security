---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: executable.science
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: executable.science
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Executable Science Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Executable Science, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Executable Science
provider_slug: executable-science
slug: executable-science-domain-security
source_filename: executable-science-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: executable.science\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: executable.science\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/executable-science/security/executable-science-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Research Library
- Datasets
- Software
- Research briefs
- AI Evaluation
- Open Science
---
