---
description: ''
domains:
- caa:
  - adns.qingcloud.com.
  dmarc: false
  dnssec: true
  domain: qingcloud.com
  spf: false
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: qingcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qingstor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QingStor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: QingStor
provider_slug: qingstor
slug: qingstor-domain-security
source_filename: qingstor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qingcloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: qingcloud.com\n  dnssec: true\n  caa:\n  - adns.qingcloud.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/qingstor/security/qingstor-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Cloud
- Infrastructure
- AI
- Storage
- Enterprise
---
