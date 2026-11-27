---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: domainroc.com
  spf: true
hosts:
- cert_expires: Jan 24 17:22:48 2027 GMT
  host: domainroc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DomainROC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DomainROC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DomainROC
provider_slug: domainroc-com
slug: domainroc-com-domain-security
source_filename: domainroc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domainroc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 17:22:48 2027 GMT\n  hsts: false\ndomains:\n- domain: domainroc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/domainroc-com/security/domainroc-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Domain
- Registration
- Cryptocurrency
- Hosting
- VPS
---
