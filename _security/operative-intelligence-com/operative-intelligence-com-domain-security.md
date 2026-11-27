---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: operative-intelligence.com
  spf: true
hosts:
- cert_expires: Jan  7 08:56:54 2027 GMT
  host: operative-intelligence.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Operative Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Operative Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Operative Intelligence
provider_slug: operative-intelligence-com
slug: operative-intelligence-com-domain-security
source_filename: operative-intelligence-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: operative-intelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 08:56:54 2027 GMT\n  hsts: false\ndomains:\n- domain: operative-intelligence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/operative-intelligence-com/security/operative-intelligence-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Automation
- Business Process
- Enterprise
- Slovenia
---
