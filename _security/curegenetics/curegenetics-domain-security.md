---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: curegenetics.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: curegenetics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curegenetics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cure Genetics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cure Genetics
provider_slug: curegenetics
slug: curegenetics-domain-security
source_filename: curegenetics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curegenetics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curegenetics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curegenetics/refs/heads/main/security/curegenetics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Gene Therapy
- Cell Therapy
- Oncology
- Genetic Disease
- Life Sciences
- China
---
