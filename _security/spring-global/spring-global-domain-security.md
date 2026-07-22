---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: springglobal.com
  spf: true
hosts:
- cert_expires: Sep 20 15:17:39 2026 GMT
  host: springglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spring Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spring Global
provider_slug: spring-global
slug: spring-global-domain-security
source_filename: spring-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: springglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:17:39 2026 GMT\n  hsts: false\ndomains:\n- domain: springglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-global/refs/heads/main/security/spring-global-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SaaS
- CPG
- Retail Execution
- Field Workforce
- Merchandising
- Artificial Intelligence
---
