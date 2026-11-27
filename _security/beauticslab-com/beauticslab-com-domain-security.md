---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beauticslab.com
  spf: false
hosts:
- cert_expires: Dec 10 20:28:53 2026 GMT
  host: beauticslab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BeauticsLab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeauticsLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: BeauticsLab
provider_slug: beauticslab-com
slug: beauticslab-com-domain-security
source_filename: beauticslab-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beauticslab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 20:28:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beauticslab.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/beauticslab-com/security/beauticslab-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Beauty
- Artificial Intelligence
- Skincare
- Market Intelligence
- Korean
---
