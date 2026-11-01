---
api_specs:
- filename: crawio-com-openapi-generated.yml
  format: yaml
  label: crawio-com API
  slug: crawio-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawio-com/openapi/_ae-authored/crawio-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crawio.com
  spf: true
hosts:
- cert_expires: Dec 13 18:04:20 2026 GMT
  host: crawio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crawio Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crawio-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: crawio-com
provider_slug: crawio-com
slug: crawio-com-domain-security
source_filename: crawio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crawio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 18:04:20 2026 GMT\n  hsts: false\ndomains:\n- domain: crawio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crawio-com/security/crawio-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web Scraping
- API
- Proxy
- Anti-Bot
- Data Extraction
---
