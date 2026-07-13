---
api_specs:
- filename: nextcloud-openapi.yml
  format: yaml
  label: Nextcloud OCS API
  slug: ocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextcloud/refs/heads/main/openapi/nextcloud-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nextcloud.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-nextcloud.example
  spf: false
hosts:
- cert_expires: Aug 12 01:03:43 2026 GMT
  host: nextcloud.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 05:49:19 2026 GMT
  host: docs.nextcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-nextcloud.example
  https: false
kind: domain-security
layout: security
method: probed
name: Nextcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nextcloud, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nextcloud
provider_slug: nextcloud
slug: nextcloud-domain-security
source_filename: nextcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nextcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 01:03:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nextcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:49:19 2026 GMT\n  hsts: false\n- host: your-nextcloud.example\n  https: false\ndomains:\n- domain: nextcloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-nextcloud.example\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextcloud/refs/heads/main/security/nextcloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Sync
- File Sharing
- Collaboration
- Self-Hosted
- Open Source
- Productivity
- WebDAV
---
