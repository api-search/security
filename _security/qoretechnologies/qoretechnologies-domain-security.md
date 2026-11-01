---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qoretechnologies.com
  spf: true
hosts:
- cert_expires: Jan  7 14:47:16 2027 GMT
  host: qoretechnologies.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qoretechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qore Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qore Technologies
provider_slug: qoretechnologies
slug: qoretechnologies-domain-security
source_filename: qoretechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qoretechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 14:47:16 2027 GMT\n  hsts: false\ndomains:\n- domain: qoretechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/qoretechnologies/security/qoretechnologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Integration
- Low-code
- Automation
- AI
- Enterprise
---
