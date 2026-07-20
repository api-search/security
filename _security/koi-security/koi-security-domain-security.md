---
api_specs:
- filename: koi-security-extensiontotal-openapi.yml
  format: yaml
  label: ExtensionTotal API
  slug: koi-security-extensiontotal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koi-security/refs/heads/main/openapi/koi-security-extensiontotal-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: koi.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: extensiontotal.com
  spf: true
hosts:
- cert_expires: Aug 27 02:44:16 2026 GMT
  host: www.koi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 15:53:10 2026 GMT
  host: app.extensiontotal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koi Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koi Security, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Koi Security
provider_slug: koi-security
slug: koi-security-domain-security
source_filename: koi-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.koi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:44:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.extensiontotal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 15:53:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: koi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: extensiontotal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koi-security/refs/heads/main/security/koi-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Endpoint Security
- Supply Chain Security
- Browser Extensions
- Developer Tools
- Threat Intelligence
- MCP Security
- Risk Scoring
---
