---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mili.eu
  spf: true
hosts:
- cert_expires: Dec 20 10:28:42 2026 GMT
  host: www.mili.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Milieu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Milieu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Milieu
provider_slug: milieu
slug: milieu-domain-security
source_filename: milieu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mili.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 10:28:42 2026 GMT\n  hsts: false\ndomains:\n- domain: mili.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/milieu/security/milieu-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Venture
- Technology
- Startup
- Europe
---
