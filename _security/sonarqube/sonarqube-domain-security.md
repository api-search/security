---
api_specs:
- filename: sonarqube-web-api-openapi.yml
  format: yaml
  label: SonarQube Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonarqube/refs/heads/main/openapi/sonarqube-web-api-openapi.yml
description: ''
domains:
- caa:
  - 128 iodef "mailto:infra@sonarsource.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sonarsource.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.sonarsource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 16:14:33 2026 GMT
  host: docs.sonarsource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonarqube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SonarQube, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SonarQube
provider_slug: sonarqube
slug: sonarqube-domain-security
source_filename: sonarqube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonarsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sonarsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:14:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sonarsource.com\n  dnssec: false\n  caa:\n  - 128 iodef \"mailto:infra@sonarsource.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonarqube/refs/heads/main/security/sonarqube-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Quality
- DevOps
- Security
- Static Analysis
---
