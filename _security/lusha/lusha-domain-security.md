---
api_specs:
- filename: openapi
  format: yaml
  label: Lusha Enrichment API
  slug: enrichment
  spec_type: OpenAPI
  url: https://docs.lusha.com/apis/openapi
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lusha.com
  spf: true
hosts:
- cert_expires: Aug 21 19:38:57 2026 GMT
  host: www.lusha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 20:35:12 2026 GMT
  host: docs.lusha.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 08:31:40 2026 GMT
  host: api.lusha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lusha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lusha, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lusha
provider_slug: lusha
slug: lusha-domain-security
source_filename: lusha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lusha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:38:57 2026 GMT\n  hsts: null\n- host: docs.lusha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:35:12 2026 GMT\n  hsts: false\n- host: api.lusha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 08:31:40 2026 GMT\n  hsts: null\ndomains:\n- domain: lusha.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/security/lusha-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sales Intelligence
- B2B
- Enrichment
- Contact Data
- Prospecting
- Intent
---
