---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: axowatch.com
  spf: true
hosts:
- cert_expires: Jan  7 17:33:28 2027 GMT
  host: axowatch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AxoWatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AxoWatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AxoWatch
provider_slug: axowatch-com
slug: axowatch-com-domain-security
source_filename: axowatch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axowatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 17:33:28 2027 GMT\n  hsts: false\ndomains:\n- domain: axowatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/axowatch-com/security/axowatch-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Monitoring
- Uptime
- Performance
- Error Tracking
- Artificial Intelligence
- Software-as-a-Service
---
