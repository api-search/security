---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: p5m.me
  spf: true
hosts:
- cert_expires: Sep 13 21:03:17 2026 GMT
  host: p5m.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: P5M Project Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for P5M Project Management, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: P5M Project Management
provider_slug: p5m-project-management
slug: p5m-project-management-domain-security
source_filename: p5m-project-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: p5m.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:03:17 2026 GMT\n  hsts: null\ndomains:\n- domain: p5m.me\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p5m-project-management/refs/heads/main/security/p5m-project-management-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
