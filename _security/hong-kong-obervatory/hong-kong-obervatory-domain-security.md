---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hko.gov.hk
  spf: true
hosts:
- cert_expires: Dec 17 08:09:55 2026 GMT
  host: www.hko.gov.hk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hong Kong Obervatory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hong Kong Obervatory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hong Kong Obervatory
provider_slug: hong-kong-obervatory
slug: hong-kong-obervatory-domain-security
source_filename: hong-kong-obervatory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hko.gov.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 08:09:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hko.gov.hk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hong-kong-obervatory/refs/heads/main/security/hong-kong-obervatory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Weather
- Public APIs
---
