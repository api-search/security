---
api_specs:
- filename: f5-distributed-cloud-services-openapi.yml
  format: yaml
  label: F5 Distributed Cloud Services API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/f5-distributed-cloud-services/refs/heads/main/openapi/f5-distributed-cloud-services-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:dnsadmin@f5.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: f5.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: volterra.io
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.f5.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: docs.cloud.f5.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 23:59:59 2026 GMT
  host: console.ves.volterra.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: F5 Distributed Cloud Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for F5 Distributed Cloud Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: F5 Distributed Cloud Services
provider_slug: f5-distributed-cloud-services
slug: f5-distributed-cloud-services-domain-security
source_filename: f5-distributed-cloud-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.f5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cloud.f5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\n- host: console.ves.volterra.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: f5.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:dnsadmin@f5.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: volterra.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5-distributed-cloud-services/refs/heads/main/security/f5-distributed-cloud-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Application Security
- Web Application Firewall
- API Security
- Multi-Cloud Networking
- DDoS Protection
- Bot Defense
- Load Balancing
- Edge Compute
---
