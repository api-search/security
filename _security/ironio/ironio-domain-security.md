---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iron.io
  spf: true
hosts:
- cert_expires: Aug 27 09:38:03 2026 GMT
  host: www.iron.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:36:18 2026 GMT
  host: dev.iron.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: mq-aws-us-east-1-1.iron.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ironio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iron.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Iron.io
provider_slug: ironio
slug: ironio-domain-security
source_filename: ironio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iron.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:38:03 2026 GMT\n  hsts: false\n- host: dev.iron.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:36:18 2026 GMT\n  hsts: false\n- host: mq-aws-us-east-1-1.iron.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: iron.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironio/refs/heads/main/security/ironio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure
- Message Queue
- Serverless
- Background Jobs
- Task Processing
- Cache
- Messaging
---
