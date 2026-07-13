---
api_specs:
- filename: tegna-audience-one-openapi.yml
  format: yaml
  label: TEGNA AudienceOne API
  slug: audience-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/openapi/tegna-audience-one-openapi.yml
- filename: tegna-premion-openapi.yml
  format: yaml
  label: TEGNA Premion OTT Advertising API
  slug: premion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/openapi/tegna-premion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tegna.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nexstar.tv
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: www.tegna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 22:43:43 2026 GMT
  host: www.nexstar.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 22:25:48 2026 GMT
  host: premion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tegna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TEGNA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TEGNA
provider_slug: tegna
slug: tegna-domain-security
source_filename: tegna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tegna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\n- host: www.nexstar.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 22:43:43 2026 GMT\n  hsts: false\n- host: premion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:25:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tegna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nexstar.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/security/tegna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcasting
- Media
- Television
- Digital Advertising
- OTT
- CTV
- Fortune 500
---
