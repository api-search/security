---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adkit.so
  spf: true
hosts:
- cert_expires: Dec 18 05:21:49 2026 GMT
  host: adkit.so
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adkit So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AdKit
provider_slug: adkit-so
slug: adkit-so-domain-security
source_filename: adkit-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adkit.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 05:21:49 2026 GMT\n  hsts: false\ndomains:\n- domain: adkit.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/adkit-so/security/adkit-so-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Marketing
- Artificial Intelligence
- AdTech
- Automation
---
