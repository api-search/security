---
api_specs:
- filename: rest-api-description
  format: yaml
  label: GitHub API
  slug: github
  spec_type: OpenAPI
  url: https://github.com/github/rest-api-description
- filename: openapi.yaml
  format: yaml
  label: GitLab API
  slug: gitlab
  spec_type: OpenAPI
  url: https://docs.gitlab.com/ee/api/openapi/openapi.yaml
- filename: swagger
  format: yaml
  label: Gitea API
  slug: gitea
  spec_type: OpenAPI
  url: https://gitea.io/api/swagger
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: git-scm.com
  spf: false
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitlab.com
  spf: true
hosts:
- cert_expires: Aug 22 09:00:38 2026 GMT
  host: git-scm.com
  hsts: false
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
name: Git Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Git, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Git
provider_slug: git
slug: git-domain-security
source_filename: git-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: git-scm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 09:00:38 2026 GMT\n  hsts: false\n- host: docs.gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:39:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: git-scm.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: gitlab.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/git/refs/heads/main/security/git-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Distributed
- Git
- Open Source
- Source Code Management
- Version Control
---
