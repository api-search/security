---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: auxiliumhealth.ca
  spf: true
hosts:
- cert_expires: Nov  3 03:33:21 2026 GMT
  host: www.auxiliumhealth.ca
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auxilium Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auxilium Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Auxilium Health
provider_slug: auxilium-health
slug: auxilium-health-domain-security
source_filename: auxilium-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auxiliumhealth.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 03:33:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: auxiliumhealth.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auxilium-health/refs/heads/main/security/auxilium-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Patient Support
- Toronto
- Canada
- Services
---
