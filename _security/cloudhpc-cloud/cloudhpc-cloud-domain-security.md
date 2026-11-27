---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudhpc.cloud
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cfdfeaservice.it
  spf: true
hosts:
- cert_expires: Jan 21 10:25:33 2027 GMT
  host: cloudhpc.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 04:36:19 2027 GMT
  host: docs.cloudhpc.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 07:09:23 2026 GMT
  host: cloud.cfdfeaservice.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cloud HPC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloud HPC, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloud HPC
provider_slug: cloudhpc-cloud
slug: cloudhpc-cloud-domain-security
source_filename: cloudhpc-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudhpc.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 10:25:33 2027 GMT\n  hsts: false\n- host: docs.cloudhpc.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 04:36:19 2027 GMT\n  hsts: false\n- host: cloud.cfdfeaservice.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:09:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudhpc.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cfdfeaservice.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cloudhpc-cloud/security/cloudhpc-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- High Performance Computing
- Cloud Computing
- Engineering Simulation
- CFD
- FEA
- CAE
- MCP
---
