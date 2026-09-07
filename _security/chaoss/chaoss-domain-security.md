---
api_specs:
- filename: chaoss-collectoss-openapi.yml
  format: yaml
  label: CollectOSS REST API
  slug: collectoss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-collectoss-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chaoss.community
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: collectoss.org
  spf: false
hosts:
- cert_expires: Dec  4 06:35:39 2026 GMT
  host: chaoss.community
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 12:59:38 2026 GMT
  host: docs.collectoss.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 15:44:43 2026 GMT
  host: www.chaoss.community
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Chaoss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CHAOSS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CHAOSS
provider_slug: chaoss
slug: chaoss-domain-security
source_filename: chaoss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaoss.community\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 06:35:39 2026 GMT\n  hsts: false\n- host: docs.collectoss.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 12:59:38 2026 GMT\n  hsts: false\n- host: www.chaoss.community\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 15:44:43 2026 GMT\n  hsts: false\ndomains:\n- domain: chaoss.community\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: collectoss.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/security/chaoss-domain-security.yml
summary_line: TLSv1.3
tags:
- Analytics
- Community Health
- DEI
- Linux Foundation
- Metrics
- Observability
- Open-Source
- Risk
- Sustainability
---
