---
api_specs:
- filename: factiva-apis
  format: yaml
  label: Factiva Snapshots API
  slug: factiva-snapshots-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Streams API
  slug: factiva-streams-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Extractions API
  slug: factiva-extractions-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Analytics API
  slug: factiva-analytics-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva DJID Taxonomy API
  slug: factiva-djid-taxonomy-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Code API
  slug: factiva-code-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dowjones.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: developer.dowjones.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.dowjones.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.dowjones.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Factiva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Factiva, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Factiva
provider_slug: factiva
slug: factiva-domain-security
source_filename: factiva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.dowjones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: false\n- host: www.dowjones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.dowjones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dowjones.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/security/factiva-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Intelligence
- Content Aggregation
- Market Data
- Media Monitoring
- News
- Research
---
