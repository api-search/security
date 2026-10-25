---
api_specs:
- filename: forcepoint-openapi-generated.yml
  format: yaml
  label: Forcepoint DLP REST API
  slug: forcepoint-dlp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forcepoint/refs/heads/main/openapi/_ae-authored/forcepoint-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: forcepoint.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: forcepoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: help.forcepoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Forcepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forcepoint, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Forcepoint
provider_slug: forcepoint
slug: forcepoint-domain-security
source_filename: forcepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forcepoint.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.forcepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: forcepoint.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forcepoint/refs/heads/main/security/forcepoint-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Security
- Data Loss Prevention
- SASE
- Security Service Edge
- Firewall
- Data Security
- Cloud Security
---
