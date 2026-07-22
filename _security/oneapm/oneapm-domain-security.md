---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oneapm.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.oneapm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: docs-ai.oneapm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Oneapm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneAPM, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OneAPM
provider_slug: oneapm
slug: oneapm-domain-security
source_filename: oneapm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oneapm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: docs-ai.oneapm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: oneapm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneapm/refs/heads/main/security/oneapm-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Application Performance Management
- APM
- Observability
- Monitoring
- AIOps
- IT Operations
- Log Analytics
- Real User Monitoring
- SaaS
---
