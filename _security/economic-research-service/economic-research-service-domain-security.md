---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.ers.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 23:20:40 2026 GMT
  host: api.ers.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Economic Research Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Economic Research Service, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Economic Research Service
provider_slug: economic-research-service
slug: economic-research-service-domain-security
source_filename: economic-research-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ers.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ers.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:20:40 2026 GMT\n  hsts: null\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/economic-research-service/refs/heads/main/security/economic-research-service-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- Economics
- Federal Government
- Research
---
