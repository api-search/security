---
api_specs:
- filename: bitbucket-cloud-rest-api-openapi.json
  format: json
  label: Bitbucket Cloud REST API
  slug: bitbucket-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/openapi/bitbucket-cloud-rest-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atlassian.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:root@bitbucket.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitbucket.org
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developer.atlassian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api.bitbucket.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitbucket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitbucket, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bitbucket
provider_slug: bitbucket
slug: bitbucket-domain-security
source_filename: bitbucket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.atlassian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bitbucket.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atlassian.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bitbucket.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:root@bitbucket.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue\
  \ \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/security/bitbucket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Atlassian
- CI/CD
- Code Collaboration
- Code Review
- DevOps
- Git
- Pull Requests
- Repository Hosting
- Version Control
---
