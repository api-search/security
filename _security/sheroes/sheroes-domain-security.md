---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sheroes.com
  spf: true
hosts:
- cert_expires: Oct  3 20:32:01 2026 GMT
  host: sheroes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sheroes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sheroes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sheroes
provider_slug: sheroes
slug: sheroes-domain-security
source_filename: sheroes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sheroes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:32:01 2026 GMT\n  hsts: false\ndomains:\n- domain: sheroes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sheroes/refs/heads/main/security/sheroes-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Community
- Social Network
- Women
- India
- Careers
- Financial Services
---
