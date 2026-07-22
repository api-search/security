---
api_specs:
- filename: xsky-xms-swagger-original.yaml
  format: yaml
  label: XSKY XMS API
  slug: xsky-xms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xsky/refs/heads/main/openapi/xsky-xms-swagger-original.yaml
description: ''
domains:
- caa:
  - xsky.com.w.kunlunaq.com.
  dmarc: false
  dnssec: true
  domain: xsky.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: xsky.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xsky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XSKY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: XSKY
provider_slug: xsky
slug: xsky-domain-security
source_filename: xsky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xsky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: xsky.com\n  dnssec: true\n  caa:\n  - xsky.com.w.kunlunaq.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xsky/refs/heads/main/security/xsky-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Storage
- Software-Defined Storage
- Object Storage
- Block Storage
- File Storage
- Data Infrastructure
- Enterprise
- China
---
