---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nervousmachine.com
  spf: false
hosts:
- cert_expires: Feb  1 19:10:20 2027 GMT
  host: nervousmachine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nervous Machine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nervous Machine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Nervous Machine
provider_slug: nervousmachine-com
slug: nervousmachine-com-domain-security
source_filename: nervousmachine-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nervousmachine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 19:10:20 2027 GMT\n  hsts: false\ndomains:\n- domain: nervousmachine.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nervousmachine-com/security/nervousmachine-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Trustworthy AI
- UncertaintyQuantification
- Data Ingestion
- InsightGeneration
---
