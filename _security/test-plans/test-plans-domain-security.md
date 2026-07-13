---
api_specs:
- filename: swagger.v3.json
  format: json
  label: Jira Software API
  slug: jira-software-api
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/jira/software/swagger.v3.json
- filename: vsts-rest-api-specs
  format: yaml
  label: Azure DevOps Test Plans API
  slug: azure-devops-test-plans-api
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: testrail.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: testrail.io
  spf: false
hosts:
- cert_expires: Aug 17 21:15:42 2026 GMT
  host: www.testrail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: yourproject.testrail.io
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developer.atlassian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Test Plans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Test Plans, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Test Plans
provider_slug: test-plans
slug: test-plans-domain-security
source_filename: test-plans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.testrail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:15:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourproject.testrail.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\n- host: developer.atlassian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: testrail.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: testrail.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-plans/refs/heads/main/security/test-plans-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documentation
- Quality Assurance
- Software Development
- Test Management
- Testing
---
