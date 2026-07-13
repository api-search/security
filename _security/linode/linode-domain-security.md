---
api_specs:
- filename: linode-api-v4-openapi.yml
  format: yaml
  label: Linode API V4
  slug: api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-api-v4-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: akamai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linode.com
  spf: true
hosts:
- cert_expires: Sep 10 06:16:17 2026 GMT
  host: techdocs.akamai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 18:51:00 2026 GMT
  host: api.linode.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: linode-api4.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for linode, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: linode
provider_slug: linode
slug: linode-domain-security
source_filename: linode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: techdocs.akamai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:16:17 2026 GMT\n  hsts: null\n- host: api.linode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 18:51:00 2026 GMT\n  hsts: null\n- host: linode-api4.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akamai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: linode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/security/linode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
