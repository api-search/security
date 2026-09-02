---
api_specs:
- filename: ubuntu-bugs-api-openapi.yml
  format: yaml
  label: Ubuntu Bugs API
  slug: ubuntu-bugs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-bugs-api-openapi.yml
- filename: ubuntu-categories-api-openapi.yml
  format: yaml
  label: Ubuntu Categories API
  slug: ubuntu-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-categories-api-openapi.yml
- filename: ubuntu-cves-api-openapi.yml
  format: yaml
  label: Ubuntu CVEs API
  slug: ubuntu-cves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-cves-api-openapi.yml
- filename: ubuntu-distributions-api-openapi.yml
  format: yaml
  label: Ubuntu Distributions API
  slug: ubuntu-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-distributions-api-openapi.yml
- filename: ubuntu-info-api-openapi.yml
  format: yaml
  label: Ubuntu Info API
  slug: ubuntu-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-info-api-openapi.yml
- filename: ubuntu-metrics-api-openapi.yml
  format: yaml
  label: Ubuntu Metrics API
  slug: ubuntu-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-metrics-api-openapi.yml
- filename: ubuntu-notices-api-openapi.yml
  format: yaml
  label: Ubuntu Notices API
  slug: ubuntu-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-notices-api-openapi.yml
- filename: ubuntu-packages-api-openapi.yml
  format: yaml
  label: Ubuntu Packages API
  slug: ubuntu-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-packages-api-openapi.yml
- filename: ubuntu-people-api-openapi.yml
  format: yaml
  label: Ubuntu People API
  slug: ubuntu-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-people-api-openapi.yml
- filename: ubuntu-projects-api-openapi.yml
  format: yaml
  label: Ubuntu Projects API
  slug: ubuntu-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-projects-api-openapi.yml
- filename: ubuntu-refresh-api-openapi.yml
  format: yaml
  label: Ubuntu Refresh API
  slug: ubuntu-refresh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-refresh-api-openapi.yml
- filename: ubuntu-search-api-openapi.yml
  format: yaml
  label: Ubuntu Search API
  slug: ubuntu-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:is-admin@canonical.com"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: launchpad.net
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:is-admin@canonical.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ubuntu.com
  spf: true
hosts:
- cert_expires: Sep 18 10:13:33 2026 GMT
  host: launchpad.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:13:33 2026 GMT
  host: api.launchpad.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 04:13:35 2026 GMT
  host: ubuntu.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubuntu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubuntu, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ubuntu
provider_slug: ubuntu
slug: ubuntu-domain-security
source_filename: ubuntu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: launchpad.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:13:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.launchpad.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:13:33 2026 GMT\n  hsts: false\n- host: ubuntu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:13:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: launchpad.net\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:is-admin@canonical.com\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ubuntu.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\
  \n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:is-admin@canonical.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/security/ubuntu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Containers
- DevOps
- Enterprise
- Linux
- Security
- Ubuntu
- Package Management
- Open-Source
---
