---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fabricdata.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: iva-api.com
  spf: false
hosts:
- cert_expires: Oct  7 15:02:06 2026 GMT
  host: www.fabricdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 12:32:13 2026 GMT
  host: knowledgebase.fabricdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: ee.iva-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fabric Origin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fabric Origin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fabric Origin
provider_slug: fabric-origin
slug: fabric-origin-domain-security
source_filename: fabric-origin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fabricdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:02:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: knowledgebase.fabricdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 12:32:13 2026 GMT\n  hsts: null\n- host: ee.iva-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fabricdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: iva-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/security/fabric-origin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Movies
- Television
- Games
- Trailers
- Metadata
---
