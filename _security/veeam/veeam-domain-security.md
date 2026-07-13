---
api_specs:
- filename: vspc-rest.html
  format: yaml
  label: Veeam Service Provider Console REST API
  slug: veeam-service-provider-console-rest-api
  spec_type: OpenAPI
  url: https://helpcenter.veeam.com/docs/vac/rest/reference/vspc-rest.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: veeam.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.veeam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: helpcenter.veeam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veeam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veeam, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Veeam
provider_slug: veeam
slug: veeam-domain-security
source_filename: veeam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: helpcenter.veeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: veeam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeam/refs/heads/main/security/veeam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backup
- Data Management
- Disaster Recovery
- Cloud Backup
- Restore
- Replication
- Data Protection
- Microsoft 365
- Azure
- Google Cloud
- Ransomware Recovery
---
