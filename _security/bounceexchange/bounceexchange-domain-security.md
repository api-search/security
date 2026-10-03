---
api_specs:
- filename: bounceexchange-openapi-generated.yml
  format: yaml
  label: Bounceexchange API
  slug: bounceexchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/openapi/_ae-authored/bounceexchange-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wunderkind.co
  spf: true
hosts:
- cert_expires: Nov 14 18:18:35 2026 GMT
  host: www.wunderkind.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bounceexchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bounceexchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bounceexchange
provider_slug: bounceexchange
slug: bounceexchange-domain-security
source_filename: bounceexchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wunderkind.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 18:18:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wunderkind.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/security/bounceexchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
