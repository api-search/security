---
api_specs:
- filename: sourceforge-admin-api-openapi.yml
  format: yaml
  label: SourceForge Admin API
  slug: sourceforge-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-admin-api-openapi.yml
- filename: sourceforge-blog-api-openapi.yml
  format: yaml
  label: SourceForge Blog API
  slug: sourceforge-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-blog-api-openapi.yml
- filename: sourceforge-discussion-api-openapi.yml
  format: yaml
  label: SourceForge Discussion API
  slug: sourceforge-discussion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-discussion-api-openapi.yml
- filename: sourceforge-projects-api-openapi.yml
  format: yaml
  label: SourceForge Projects API
  slug: sourceforge-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-projects-api-openapi.yml
- filename: sourceforge-tracker-api-openapi.yml
  format: yaml
  label: SourceForge Tracker API
  slug: sourceforge-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-tracker-api-openapi.yml
- filename: sourceforge-users-api-openapi.yml
  format: yaml
  label: SourceForge Users API
  slug: sourceforge-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-users-api-openapi.yml
- filename: sourceforge-wikis-api-openapi.yml
  format: yaml
  label: SourceForge Wikis API
  slug: sourceforge-wikis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/openapi/sourceforge-wikis-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:siteops@slashdotmedia.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sourceforge.net
  spf: true
hosts:
- cert_expires: Aug 26 01:39:43 2026 GMT
  host: sourceforge.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourceforge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SourceForge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SourceForge
provider_slug: sourceforge
slug: sourceforge-domain-security
source_filename: sourceforge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sourceforge.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:39:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sourceforge.net\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:siteops@slashdotmedia.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourceforge/refs/heads/main/security/sourceforge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Source
- Developer Tools
- Project Management
- Code Hosting
- Collaboration
---
