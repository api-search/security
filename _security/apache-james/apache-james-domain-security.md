---
api_specs:
- filename: apache-james-domains-api-openapi.yml
  format: yaml
  label: Apache James Domains API
  slug: apache-james-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-domains-api-openapi.yml
- filename: apache-james-healthcheck-api-openapi.yml
  format: yaml
  label: Apache James HealthCheck API
  slug: apache-james-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-healthcheck-api-openapi.yml
- filename: apache-james-mailboxes-api-openapi.yml
  format: yaml
  label: Apache James Mailboxes API
  slug: apache-james-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-mailboxes-api-openapi.yml
- filename: apache-james-mailqueues-api-openapi.yml
  format: yaml
  label: Apache James MailQueues API
  slug: apache-james-mailqueues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-mailqueues-api-openapi.yml
- filename: apache-james-mailrepositories-api-openapi.yml
  format: yaml
  label: Apache James MailRepositories API
  slug: apache-james-mailrepositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-mailrepositories-api-openapi.yml
- filename: apache-james-quotas-api-openapi.yml
  format: yaml
  label: Apache James Quotas API
  slug: apache-james-quotas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-quotas-api-openapi.yml
- filename: apache-james-tasks-api-openapi.yml
  format: yaml
  label: Apache James Tasks API
  slug: apache-james-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-tasks-api-openapi.yml
- filename: apache-james-users-api-openapi.yml
  format: yaml
  label: Apache James Users API
  slug: apache-james-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: james.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache James Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache James, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache James
provider_slug: apache-james
slug: apache-james-domain-security
source_filename: apache-james-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: james.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/security/apache-james-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
---
