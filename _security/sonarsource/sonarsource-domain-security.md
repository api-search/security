---
api_specs:
- filename: sonarsource-web-api-openapi.yml
  format: yaml
  label: SonarQube Cloud Web API
  slug: sonarqube-cloud-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonarsource/refs/heads/main/openapi/sonarsource-web-api-openapi.yml
description: ''
domains:
- caa:
  - 128 iodef "mailto:infra@sonarsource.com"
  - 0 issue "amazon.com"
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sonarsource.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazontrust.com"
  - 128 iodef "mailto:infra@sonarsource.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sonarcloud.io
  spf: true
hosts:
- cert_expires: Oct  9 16:14:33 2026 GMT
  host: docs.sonarsource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: sonarcloud.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonarsource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SonarSource, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SonarSource
provider_slug: sonarsource
slug: sonarsource-domain-security
source_filename: sonarsource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.sonarsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:14:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sonarcloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sonarsource.com\n  dnssec: false\n  caa:\n  - 128 iodef \"mailto:infra@sonarsource.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sonarcloud.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazontrust.com\"\n  - 128 iodef \"mailto:infra@sonarsource.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonarsource/refs/heads/main/security/sonarsource-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Code Quality
- Static Analysis
- Code Security
- SAST
- Developer Tools
- DevOps
- Code Review
- SonarQube
---
