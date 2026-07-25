---
api_specs:
- filename: jenkins-computer-api-openapi.yml
  format: yaml
  label: Jenkins Computer API
  slug: jenkins-computer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/openapi/jenkins-computer-api-openapi.yml
- filename: jenkins-jobs-api-openapi.yml
  format: yaml
  label: Jenkins Jobs API
  slug: jenkins-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/openapi/jenkins-jobs-api-openapi.yml
- filename: jenkins-queue-api-openapi.yml
  format: yaml
  label: Jenkins Queue API
  slug: jenkins-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/openapi/jenkins-queue-api-openapi.yml
- filename: jenkins-server-api-openapi.yml
  format: yaml
  label: Jenkins Server API
  slug: jenkins-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/openapi/jenkins-server-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jenkins.io
  spf: true
hosts:
- cert_expires: Aug 19 21:52:45 2026 GMT
  host: www.jenkins.io
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jenkins Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jenkins, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jenkins
provider_slug: jenkins
slug: jenkins-domain-security
source_filename: jenkins-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jenkins.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 19 21:52:45 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: jenkins.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/security/jenkins-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Automation
- Build Server
- CI/CD
- Continuous Delivery
- Continuous Integration
- DevOps
- Open Source
- Remote Access API
---
