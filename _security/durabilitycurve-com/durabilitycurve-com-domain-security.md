---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: durabilitycurve.com
  spf: true
hosts:
- cert_expires: Jan 15 07:14:35 2027 GMT
  host: durabilitycurve.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Durability Curve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Durability Curve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: The Durability Curve
provider_slug: durabilitycurve-com
slug: durabilitycurve-com-domain-security
source_filename: durabilitycurve-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: durabilitycurve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 07:14:35 2027 GMT\n  hsts: false\ndomains:\n- domain: durabilitycurve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/durabilitycurve-com/security/durabilitycurve-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Tools
- Essays
- Open Source
---
