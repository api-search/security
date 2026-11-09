---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: applaunchflow.com
  spf: true
hosts:
- cert_expires: Jan 17 14:34:44 2027 GMT
  host: applaunchflow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Applaunchflow Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppLaunchFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppLaunchFlow
provider_slug: applaunchflow-com
slug: applaunchflow-com-domain-security
source_filename: applaunchflow-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: applaunchflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 14:34:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: applaunchflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/applaunchflow-com/security/applaunchflow-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software-as-a-Service
- Marketing
- Artificial Intelligence
- Asset Generation
---
