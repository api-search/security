---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: usehalo.com
  spf: true
hosts:
- cert_expires: Jan 23 17:01:45 2027 GMT
  host: usehalo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Halopsa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HaloPSA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HaloPSA
provider_slug: halopsa
slug: halopsa-domain-security
source_filename: halopsa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usehalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 17:01:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usehalo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/halopsa/security/halopsa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Workflow Automation
- IT Service Management
- Customer Service Management
- Enterprise Service Management
---
