---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: csa-iot.org
  spf: true
hosts:
- cert_expires: Dec 25 03:20:00 2026 GMT
  host: csa-iot.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connectivity Standards Alliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connectivity Standards Alliance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Connectivity Standards Alliance
provider_slug: connectivity-standards-alliance
slug: connectivity-standards-alliance-domain-security
source_filename: connectivity-standards-alliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: csa-iot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 03:20:00 2026 GMT\n  hsts: false\ndomains:\n- domain: csa-iot.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connectivity-standards-alliance/refs/heads/main/security/connectivity-standards-alliance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IoT
- Standards
- Consortium
- Open Source
---
