---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: splunk.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.splunk.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 01:57:37 2026 GMT
  host: help.splunk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Splunk Soar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splunk SOAR, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Splunk SOAR
provider_slug: splunk-soar
slug: splunk-soar-domain-security
source_filename: splunk-soar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.splunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: help.splunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 01:57:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: splunk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splunk-soar/refs/heads/main/security/splunk-soar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- SOAR
- Automation
- Orchestration
- Incident Response
- SOC
- Security Operations
- Playbooks
- Case Management
- Threat Intelligence
---
