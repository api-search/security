---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dynatronsoftware.com
  spf: true
hosts:
- cert_expires: Jan 30 21:34:40 2027 GMT
  host: dynatronsoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dynatron Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynatron Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dynatron Software
provider_slug: dynatron
slug: dynatron-domain-security
source_filename: dynatron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dynatronsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 21:34:40 2027 GMT\n  hsts: false\ndomains:\n- domain: dynatronsoftware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dynatron/security/dynatron-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Automotive
- Fixed Ops
- Artificial Intelligence
- Data Analytics
- Software-as-a-Service
---
