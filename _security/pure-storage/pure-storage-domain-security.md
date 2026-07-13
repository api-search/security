---
api_specs:
- filename: flasharray-rest-api-openapi.yml
  format: yaml
  label: FlashArray REST API
  slug: flasharray-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pure-storage/refs/heads/main/openapi/flasharray-rest-api-openapi.yml
- filename: flashblade-rest-api-openapi.yml
  format: yaml
  label: FlashBlade REST API
  slug: flashblade-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pure-storage/refs/heads/main/openapi/flashblade-rest-api-openapi.yml
- filename: pure1-cloud-api-openapi.yml
  format: yaml
  label: Pure1 Public REST API
  slug: pure1-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pure-storage/refs/heads/main/openapi/pure1-cloud-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: purestorage.com
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: portworx.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.purestorage.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 06:24:19 2026 GMT
  host: code.purestorage.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 08:30:36 2026 GMT
  host: docs.portworx.com
  hsts: true
  hsts_max_age: 7257600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pure Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pure Storage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pure Storage
provider_slug: pure-storage
slug: pure-storage-domain-security
source_filename: pure-storage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.purestorage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: code.purestorage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:24:19 2026 GMT\n  hsts: false\n- host: docs.portworx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 08:30:36 2026 GMT\n  hsts: true\n  hsts_max_age: 7257600\ndomains:\n- domain: purestorage.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: portworx.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\
  \n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pure-storage/refs/heads/main/security/pure-storage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Storage
- Data Storage
- Flash Storage
- Enterprise Storage
- Cloud Storage
- Object Storage
- File Storage
- Block Storage
- Kubernetes Storage
- Infrastructure
---
