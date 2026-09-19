---
api_specs:
- filename: iab-tech-lab-opendirect-1-5-1-swagger.yaml
  format: yaml
  label: OpenDirect API
  slug: opendirect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml
- filename: iab-tech-lab-agentic-advertising-api-openapi.yaml
  format: yaml
  label: IAB Agentic Advertising API
  slug: agentic-advertising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-agentic-advertising-api-openapi.yaml
- filename: iab-tech-lab-seller-agent-openapi.json
  format: json
  label: Seller Agent API
  slug: seller-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-seller-agent-openapi.json
- filename: iab-tech-lab-buyer-agent-openapi.json
  format: json
  label: Buyer Agent API
  slug: buyer-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-buyer-agent-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iabtechlab.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: iabtechlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:24:21 2026 GMT
  host: tools.iabtechlab.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.iabtechlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Iab Tech Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IAB Tech Lab, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IAB Tech Lab
provider_slug: iab-tech-lab
slug: iab-tech-lab-domain-security
source_filename: iab-tech-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iabtechlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tools.iabtechlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:24:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.iabtechlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iabtechlab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/security/iab-tech-lab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Standards
- Programmatic
- Real-Time Bidding
- Consent
- Privacy
- Video Ads
- Agentic Advertising
- Non-Profit
---
