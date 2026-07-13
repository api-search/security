---
api_specs:
- filename: puppet-openapi.yml
  format: yaml
  label: Puppet Enterprise Orchestrator API
  slug: orchestrator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puppet/refs/heads/main/openapi/puppet-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: puppet.com
  spf: true
hosts:
- cert_expires: Aug 24 08:33:21 2026 GMT
  host: www.puppet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: help.puppet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: forge.puppet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Puppet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puppet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Puppet
provider_slug: puppet
slug: puppet-domain-security
source_filename: puppet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.puppet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:33:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.puppet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: forge.puppet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: puppet.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puppet/refs/heads/main/security/puppet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Configuration Management
- DevOps
- Enterprise
- Infrastructure as Code
- Orchestration
- RBAC
---
