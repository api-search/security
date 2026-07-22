---
api_specs:
- filename: puppet-labs-forge-openapi-original.json
  format: json
  label: Puppet Forge v3 API
  slug: puppet-forge-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puppet-labs/refs/heads/main/openapi/puppet-labs-forge-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "awstrust.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
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
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: forgeapi.puppet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Puppet Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puppet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Puppet
provider_slug: puppet-labs
slug: puppet-labs-domain-security
source_filename: puppet-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.puppet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:33:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: forgeapi.puppet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: puppet.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puppet-labs/refs/heads/main/security/puppet-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Infrastructure Automation
- Configuration Management
- DevOps
- Module Registry
- Compliance
---
