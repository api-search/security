---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: suppfusion.com
  spf: true
hosts:
- cert_expires: Jan 15 08:32:21 2027 GMT
  host: suppfusion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Suppfusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Support Fusion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Support Fusion
provider_slug: suppfusion
slug: suppfusion-domain-security
source_filename: suppfusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suppfusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 08:32:21 2027 GMT\n  hsts: false\ndomains:\n- domain: suppfusion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/suppfusion/security/suppfusion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IT
- Integration
- Collaboration
- Support
---
