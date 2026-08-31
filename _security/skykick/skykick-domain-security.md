---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: connectwise.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Oct  5 17:52:43 2026 GMT
  host: www.connectwise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 02:49:57 2027 GMT
  host: skykick.developer.azure-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: apis.cloudservices.connectwise.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skykick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SkyKick, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SkyKick
provider_slug: skykick
slug: skykick-domain-security
source_filename: skykick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.connectwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:52:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: skykick.developer.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 02:49:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apis.cloudservices.connectwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: connectwise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skykick/refs/heads/main/security/skykick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Backup
- Migration
- Microsoft 365
- Managed Service Providers
- SaaS Security
- Cloud Automation
- Data Protection
- Azure API Management
---
