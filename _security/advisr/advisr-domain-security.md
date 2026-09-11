---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: advisr.com
  spf: true
hosts:
- cert_expires: Nov  7 21:05:14 2026 GMT
  host: www.advisr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 17:37:47 2026 GMT
  host: apidocs.advisr.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:25:35 2026 GMT
  host: api.advisr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Advisr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advisr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Advisr
provider_slug: advisr
slug: advisr-domain-security
source_filename: advisr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.advisr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 21:05:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.advisr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 17:37:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.advisr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:25:35 2026 GMT\n  hsts: null\ndomains:\n- domain: advisr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advisr/refs/heads/main/security/advisr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Media
- Sales
- Sales Enablement
- Media Planning
- Proposals
- Advertising Sales
- Campaigns
- CRM
---
