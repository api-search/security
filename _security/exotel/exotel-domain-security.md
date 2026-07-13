---
api_specs:
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Voice Call API
  slug: exotel-voice-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Call Details API
  slug: exotel-call-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel SMS API
  slug: exotel-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Numbers API
  slug: exotel-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Campaigns API
  slug: exotel-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-asyncapi.yml
  format: yaml
  label: Exotel AgentStream Voice Streaming API
  slug: exotel-agentstream-voice-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/asyncapi/exotel-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:itadmin@exotel.com"
  dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: mailto:team-it@exotel.com
  dnssec: false
  domain: exotel.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:spf.secure.ravenmail.io include:aspmx.pardot.com include:stspg-customer.com -all
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M04
  cert_not_before: Apr 17 00:00:00 2026 GMT
  host: exotel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  server: nginx/1.28.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M04
  cert_not_before: Jun 15 00:00:00 2026 GMT
  host: api.exotel.com
  hsts: false
  https: true
  notes: API host (Singapore cluster). Returns HTTP 400 to an unauthenticated root request, as expected for a credentialed API base.
  server: Apache
- cert_expires: Oct 16 23:59:59 2026 GMT
  cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M04
  cert_not_before: Apr  2 00:00:00 2026 GMT
  host: developer.exotel.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  server: Vercel
kind: domain-security
layout: security
method: probed
name: Exotel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exotel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Exotel
provider_slug: exotel
slug: exotel-domain-security
source_filename: exotel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API/docs hosts\nhosts:\n- host: exotel.com\n  https: true\n  cert_issuer: 'C=US, O=Amazon, CN=Amazon RSA 2048 M04'\n  cert_not_before: Apr 17 00:00:00 2026 GMT\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  server: nginx/1.28.3\n- host: api.exotel.com\n  https: true\n  cert_issuer: 'C=US, O=Amazon, CN=Amazon RSA 2048 M04'\n  cert_not_before: Jun 15 00:00:00 2026 GMT\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n  server: Apache\n  notes: >-\n    API host (Singapore cluster). Returns HTTP 400 to an unauthenticated\n    root request, as expected for a credentialed API base.\n- host: developer.exotel.com\n  https: true\n  cert_issuer: 'C=US, O=Amazon, CN=Amazon RSA 2048 M04'\n  cert_not_before: Apr  2 00:00:00 2026 GMT\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload:\
  \ true\n  server: Vercel\ndomains:\n- domain: exotel.com\n  dnssec: false\n  caa:\n  - '0 issue \"letsencrypt.org\"'\n  - '0 issue \"amazon.com\"'\n  - '0 issuewild \"amazon.com\"'\n  - '0 issuewild \"letsencrypt.org\"'\n  - '0 iodef \"mailto:itadmin@exotel.com\"'\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:_spf.salesforce.com include:spf.secure.ravenmail.io include:aspmx.pardot.com include:stspg-customer.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: 'mailto:team-it@exotel.com'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/security/exotel-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Cloud Telephony
- Voice
- SMS
- India
- CPaaS
- Call Center
- IVR
- Numbers
- Communications
- Customer Engagement
---
