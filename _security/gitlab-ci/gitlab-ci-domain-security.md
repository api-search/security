---
api_specs:
- filename: gitlab-ci-openapi.yml
  format: yaml
  label: GitLab REST API v4 (CI/CD endpoints)
  slug: rest-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab-ci/refs/heads/main/openapi/gitlab-ci-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@gitlab.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitlab.com
  spf: true
hosts:
- cert_expires: Aug 18 18:49:38 2026 GMT
  host: about.gitlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 12:39:50 2026 GMT
  host: docs.gitlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: gitlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitlab Ci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitLab CI/CD, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GitLab CI/CD
provider_slug: gitlab-ci
slug: gitlab-ci-domain-security
source_filename: gitlab-ci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: about.gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 18:49:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:39:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gitlab.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@gitlab.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab-ci/refs/heads/main/security/gitlab-ci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DevOps
- CI/CD
- Pipelines
- GitLab
- DevSecOps
- Runners
- Container Registry
---
