---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: enterpriseintegrationpatterns.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: www.enterpriseintegrationpatterns.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enterprise Integration Patterns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enterprise Integration Patterns, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Enterprise Integration Patterns
provider_slug: enterprise-integration-patterns
slug: enterprise-integration-patterns-domain-security
source_filename: enterprise-integration-patterns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enterpriseintegrationpatterns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: enterpriseintegrationpatterns.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enterprise-integration-patterns/refs/heads/main/security/enterprise-integration-patterns-domain-security.yml
summary_line: TLSv1.3
tags:
- Architecture
- Design Patterns
- Enterprise
- Integration
- Messaging
---
