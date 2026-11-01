---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ufl.edu
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: dcp.ufl.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: University Of Florida Florida Institute For Built Environment Resilience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Florida, Florida Institute for Built Environment Resilience, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Florida, Florida Institute for Built Environment Resilience
provider_slug: university-of-florida-florida-institute-for-built-environment-resilience
slug: university-of-florida-florida-institute-for-built-environment-resilience-domain-security
source_filename: university-of-florida-florida-institute-for-built-environment-resilience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dcp.ufl.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ufl.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/university-of-florida-florida-institute-for-built-environment-resilience/security/university-of-florida-florida-institute-for-built-environment-resilience-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Research
- Climate-Resilience
- Engineering
- Education
---
