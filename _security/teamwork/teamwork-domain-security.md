---
api_specs:
- filename: download
  format: yaml
  label: Teamwork.com Projects API v3
  slug: projects-api-v3
  spec_type: OpenAPI
  url: https://apidocs.teamwork.com/api/oas/download?slug=teamwork&api_version=v3
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teamwork.com
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: www.teamwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 16:28:12 2026 GMT
  host: apidocs.teamwork.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teamwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teamwork.com, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Teamwork.com
provider_slug: teamwork
slug: teamwork-domain-security
source_filename: teamwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teamwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.teamwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:28:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: teamwork.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamwork/refs/heads/main/security/teamwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Project Management
- Client Services
- Task Management
- Time Tracking
- Collaboration
- Professional Services Automation
---
