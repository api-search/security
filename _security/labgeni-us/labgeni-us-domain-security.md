---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: labgeni.us
  spf: true
hosts:
- cert_expires: Dec 30 17:32:25 2026 GMT
  host: labgeni.us
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Labgeni Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LabGenius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LabGenius
provider_slug: labgeni-us
slug: labgeni-us-domain-security
source_filename: labgeni-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: labgeni.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 17:32:25 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: labgeni.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/labgeni-us/security/labgeni-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- AI
- AntibodyDiscovery
- Therapeutics
- MachineLearning
---
