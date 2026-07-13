---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: standards.rest
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zalando.com
  spf: true
hosts:
- cert_expires: Sep  7 17:16:51 2026 GMT
  host: standards.rest
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 21:17:50 2026 GMT
  host: opensource.zalando.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restful Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RESTful Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RESTful Services
provider_slug: restful-services
slug: restful-services-domain-security
source_filename: restful-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standards.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 17:16:51 2026 GMT\n  hsts: false\n- host: opensource.zalando.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:17:50 2026 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: standards.rest\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: zalando.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restful-services/refs/heads/main/security/restful-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Architecture
- HTTP
- Microservices
- REST
- Web Services
---
