---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: construcompany.com.br
  spf: true
hosts:
- cert_expires: Nov 30 10:29:55 2026 GMT
  host: www.construcompany.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Constru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Constru
provider_slug: constru
slug: constru-domain-security
source_filename: constru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.construcompany.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 10:29:55 2026 GMT\n  hsts: false\ndomains:\n- domain: construcompany.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constru/refs/heads/main/security/constru-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Construction
- Real Estate
- Brazil
- Infrastructure
---
