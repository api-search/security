---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sesamesoftware.com
  spf: true
hosts:
- cert_expires: Dec 23 10:36:10 2026 GMT
  host: sesamesoftware.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sesamesoftware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sesame Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sesame Software
provider_slug: sesamesoftware
slug: sesamesoftware-domain-security
source_filename: sesamesoftware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sesamesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 10:36:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: sesamesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sesamesoftware/security/sesamesoftware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Backup
- Data Replication
- Data Migration
- Data Integration
- Enterprise Data Management
- Salesforce
- NetSuite
---
