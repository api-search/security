---
api_specs:
- filename: td-synnex-streamone-ion-openapi.yml
  format: yaml
  label: TD SYNNEX StreamOne Ion API
  slug: streamone-ion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-streamone-ion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tdsynnex.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: streamone.cloud
  spf: true
hosts:
- cert_expires: Nov 11 11:31:17 2026 GMT
  host: www.tdsynnex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 11:01:06 2026 GMT
  host: docs.streamone.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 16:53:40 2026 GMT
  host: ion.tdsynnex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Td Synnex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TD SYNNEX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TD SYNNEX
provider_slug: td-synnex
slug: td-synnex-domain-security
source_filename: td-synnex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tdsynnex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 11:31:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.streamone.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:01:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ion.tdsynnex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 16:53:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tdsynnex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: streamone.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/security/td-synnex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Technology Distribution
- IT Distribution
- Cloud
- Reseller
- StreamOne
- Fortune 100
- B2B
---
