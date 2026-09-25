---
api_specs:
- filename: greif-wp-json-discovery.json
  format: json
  label: Greif Website (WordPress REST)
  slug: greif-com-website-wordpress-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greif/refs/heads/main/openapi/greif-wp-json-discovery.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greif.com
  spf: true
hosts:
- cert_expires: Nov 12 23:38:12 2026 GMT
  host: www.greif.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Greif Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greif, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Greif
provider_slug: greif
slug: greif-domain-security
source_filename: greif-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greif.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:38:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: greif.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greif/refs/heads/main/security/greif-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Packaging
- Industrial
- Manufacturing
- Sustainability
- Fortune 1000
---
