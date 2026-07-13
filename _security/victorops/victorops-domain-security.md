---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: splunk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: victorops.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.splunk.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: help.victorops.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.victorops.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Victorops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splunk On-Call (VictorOps), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Splunk On-Call (VictorOps)
provider_slug: victorops
slug: victorops-domain-security
source_filename: victorops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.splunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: help.victorops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.victorops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: splunk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: victorops.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/victorops/refs/heads/main/security/victorops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Incident Management
- On-Call
- Alerting
- DevOps
- SRE
- Incident Response
- Observability
---
