---
api_specs:
- filename: sitefinity-cms-content-api-openapi.yml
  format: yaml
  label: Sitefinity CMS Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitefinity-cms/refs/heads/main/openapi/sitefinity-cms-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: progress.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sitefinity.com
  spf: true
hosts:
- cert_expires: Sep 11 20:55:58 2026 GMT
  host: www.progress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-site.sitefinity.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sitefinity Cms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sitefinity CMS, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sitefinity CMS
provider_slug: sitefinity-cms
slug: sitefinity-cms-domain-security
source_filename: sitefinity-cms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.progress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:55:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-site.sitefinity.com\n  https: false\ndomains:\n- domain: progress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sitefinity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitefinity-cms/refs/heads/main/security/sitefinity-cms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content Management
- Headless CMS
- .NET
- REST
---
