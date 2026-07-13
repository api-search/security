---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: luraproject.org
  spf: false
hosts:
- cert_expires: Sep 30 18:43:47 2026 GMT
  host: luraproject.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lura Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lura Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lura Project
provider_slug: lura-project
slug: lura-project-domain-security
source_filename: lura-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luraproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:43:47 2026 GMT\n  hsts: false\ndomains:\n- domain: luraproject.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lura-project/refs/heads/main/security/lura-project-domain-security.yml
summary_line: TLSv1.3
tags:
- API Gateway
- Go
- Linux Foundation
- Microservices
- Open Source
---
