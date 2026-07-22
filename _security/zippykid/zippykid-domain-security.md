---
api_specs:
- filename: zippykid-pressable-openapi-original.json
  format: json
  label: Pressable API
  slug: pressable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zippykid/refs/heads/main/openapi/zippykid-pressable-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pressable.com
  spf: true
hosts:
- cert_expires: Sep 22 01:13:16 2026 GMT
  host: pressable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 19:45:16 2026 GMT
  host: my.pressable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zippykid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZippyKid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ZippyKid
provider_slug: zippykid
slug: zippykid-domain-security
source_filename: zippykid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pressable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:13:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.pressable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:45:16 2026 GMT\n  hsts: null\ndomains:\n- domain: pressable.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zippykid/refs/heads/main/security/zippykid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- WordPress
- Managed Hosting
- WordPress Hosting
- Web Hosting
- WP Cloud
- MCP
- DevOps
---
