---
api_specs:
- filename: amazon-connect-agent-statuses-api-openapi.yml
  format: yaml
  label: Amazon Connect Agent Statuses API
  slug: amazon-connect-agent-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-agent-statuses-api-openapi.yml
- filename: amazon-connect-authentication-api-openapi.yml
  format: yaml
  label: Amazon Connect Authentication API
  slug: amazon-connect-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-authentication-api-openapi.yml
- filename: amazon-connect-contact-flows-api-openapi.yml
  format: yaml
  label: Amazon Connect Contact Flows API
  slug: amazon-connect-contact-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-contact-flows-api-openapi.yml
- filename: amazon-connect-contacts-api-openapi.yml
  format: yaml
  label: Amazon Connect Contacts API
  slug: amazon-connect-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-contacts-api-openapi.yml
- filename: amazon-connect-hours-of-operations-api-openapi.yml
  format: yaml
  label: Amazon Connect Hours of Operations API
  slug: amazon-connect-hours-of-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-hours-of-operations-api-openapi.yml
- filename: amazon-connect-instances-api-openapi.yml
  format: yaml
  label: Amazon Connect Instances API
  slug: amazon-connect-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-instances-api-openapi.yml
- filename: amazon-connect-metrics-api-openapi.yml
  format: yaml
  label: Amazon Connect Metrics API
  slug: amazon-connect-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-metrics-api-openapi.yml
- filename: amazon-connect-queues-api-openapi.yml
  format: yaml
  label: Amazon Connect Queues API
  slug: amazon-connect-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-queues-api-openapi.yml
- filename: amazon-connect-routing-profiles-api-openapi.yml
  format: yaml
  label: Amazon Connect Routing Profiles API
  slug: amazon-connect-routing-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-routing-profiles-api-openapi.yml
- filename: amazon-connect-security-profiles-api-openapi.yml
  format: yaml
  label: Amazon Connect Security Profiles API
  slug: amazon-connect-security-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-security-profiles-api-openapi.yml
- filename: amazon-connect-tags-api-openapi.yml
  format: yaml
  label: Amazon Connect Tags API
  slug: amazon-connect-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-tags-api-openapi.yml
- filename: amazon-connect-users-api-openapi.yml
  format: yaml
  label: Amazon Connect Users API
  slug: amazon-connect-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/openapi/amazon-connect-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: connect.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Connect, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Connect
provider_slug: amazon-connect
slug: amazon-connect-domain-security
source_filename: amazon-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: connect.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/security/amazon-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- Artificial Intelligence
- Omnichannel
---
