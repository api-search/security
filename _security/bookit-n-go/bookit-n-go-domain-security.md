---
api_specs:
- filename: bookit-n-go-agent-api-openapi.yml
  format: yaml
  label: Bookit N Go Agent API
  slug: bookit-n-go-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-agent-api-openapi.yml
- filename: bookit-n-go-flights-api-openapi.yml
  format: yaml
  label: Bookit N Go Flights API
  slug: bookit-n-go-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-flights-api-openapi.yml
- filename: bookit-n-go-hotels-api-openapi.yml
  format: yaml
  label: Bookit N Go Hotels API
  slug: bookit-n-go-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-hotels-api-openapi.yml
- filename: bookit-n-go-travelers-api-openapi.yml
  format: yaml
  label: Bookit N Go Travelers API
  slug: bookit-n-go-travelers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-travelers-api-openapi.yml
- filename: bookit-n-go-trips-api-openapi.yml
  format: yaml
  label: Bookit N Go Trips API
  slug: bookit-n-go-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-trips-api-openapi.yml
- filename: bookit-n-go-webhooks-api-openapi.yml
  format: yaml
  label: Bookit N Go Webhooks API
  slug: bookit-n-go-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bookitngo.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.bookitngo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bookit N Go Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bookit N Go, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bookit N Go
provider_slug: bookit-n-go
slug: bookit-n-go-domain-security
source_filename: bookit-n-go-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bookitngo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bookitngo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/security/bookit-n-go-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- SaaS
- AI
- White-label
- B2B
---
