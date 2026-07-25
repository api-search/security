---
api_specs:
- filename: sublime-security-binexplode-api-openapi.yml
  format: yaml
  label: Sublime Security BinExplode API
  slug: sublime-security-binexplode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-binexplode-api-openapi.yml
- filename: sublime-security-email-bombs-api-openapi.yml
  format: yaml
  label: Sublime Security Email Bombs API
  slug: sublime-security-email-bombs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-email-bombs-api-openapi.yml
- filename: sublime-security-enrichment-api-openapi.yml
  format: yaml
  label: Sublime Security Enrichment API
  slug: sublime-security-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-enrichment-api-openapi.yml
- filename: sublime-security-events-in-the-audit-log-api-openapi.yml
  format: yaml
  label: Sublime Security Events in the audit log API
  slug: sublime-security-events-in-the-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-events-in-the-audit-log-api-openapi.yml
- filename: sublime-security-hunt-jobs-api-openapi.yml
  format: yaml
  label: Sublime Security Hunt Jobs API
  slug: sublime-security-hunt-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-hunt-jobs-api-openapi.yml
- filename: sublime-security-lists-api-openapi.yml
  format: yaml
  label: Sublime Security Lists API
  slug: sublime-security-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-lists-api-openapi.yml
- filename: sublime-security-live-flow-api-openapi.yml
  format: yaml
  label: Sublime Security Live flow API
  slug: sublime-security-live-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-live-flow-api-openapi.yml
- filename: sublime-security-mailboxes-api-openapi.yml
  format: yaml
  label: Sublime Security Mailboxes API
  slug: sublime-security-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-mailboxes-api-openapi.yml
- filename: sublime-security-message-groups-api-openapi.yml
  format: yaml
  label: Sublime Security Message Groups API
  slug: sublime-security-message-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-message-groups-api-openapi.yml
- filename: sublime-security-messages-api-openapi.yml
  format: yaml
  label: Sublime Security Messages API
  slug: sublime-security-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-messages-api-openapi.yml
- filename: sublime-security-organizations-api-openapi.yml
  format: yaml
  label: Sublime Security Organizations API
  slug: sublime-security-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-organizations-api-openapi.yml
- filename: sublime-security-roles-api-openapi.yml
  format: yaml
  label: Sublime Security Roles API
  slug: sublime-security-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-roles-api-openapi.yml
- filename: sublime-security-rules-api-openapi.yml
  format: yaml
  label: Sublime Security Rules API
  slug: sublime-security-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-rules-api-openapi.yml
- filename: sublime-security-scim-api-openapi.yml
  format: yaml
  label: Sublime Security SCIM API
  slug: sublime-security-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-scim-api-openapi.yml
- filename: sublime-security-tasks-api-openapi.yml
  format: yaml
  label: Sublime Security Tasks API
  slug: sublime-security-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-tasks-api-openapi.yml
- filename: sublime-security-user-reports-api-openapi.yml
  format: yaml
  label: Sublime Security User Reports API
  slug: sublime-security-user-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-user-reports-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sublime.security
  spf: true
hosts:
- cert_expires: Oct 12 05:06:58 2026 GMT
  host: sublime.security
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sublime Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sublime Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sublime Security
provider_slug: sublime-security
slug: sublime-security-domain-security
source_filename: sublime-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sublime.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:06:58 2026 GMT\n  hsts: null\ndomains:\n- domain: sublime.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/security/sublime-security-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Email Security
- Phishing
- Detection as Code
- Threat Detection
- Cloud Email Security
- SCIM
---
