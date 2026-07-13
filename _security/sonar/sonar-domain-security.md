---
api_specs:
- filename: sonar-sonarcloud-api-openapi.yml
  format: yaml
  label: SonarCloud API
  slug: sonarcloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/openapi/sonar-sonarcloud-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 128 iodef "mailto:infra@sonarsource.com"
  - 0 issue "digicert.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sonarsource.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "amazontrust.com"
  - 0 issue "digicert.com"
  - 128 iodef "mailto:infra@sonarsource.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sonarcloud.io
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
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: sonarcloud.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sonar
provider_slug: sonar
slug: sonar-domain-security
source_filename: sonar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonarsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sonarsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:14:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sonarcloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sonarsource.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 128 iodef \"mailto:infra@sonarsource.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sonarcloud.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\
  \n  - 0 issue \"digicert.com\"\n  - 128 iodef \"mailto:infra@sonarsource.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonar/refs/heads/main/security/sonar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Code Quality
- DevOps
- Security
- SonarCloud
- SonarQube
- Static Analysis
---
