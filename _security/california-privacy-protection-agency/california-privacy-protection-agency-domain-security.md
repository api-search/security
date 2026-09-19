---
api_specs:
- filename: california-privacy-protection-agency-drop-data-broker-api-openapi.yml
  format: yaml
  label: DROP Data Broker API
  slug: drop-data-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/california-privacy-protection-agency/refs/heads/main/openapi/california-privacy-protection-agency-drop-data-broker-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ca.gov
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: cppa.ca.gov
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 11 03:16:02 2026 GMT
  host: privacy.ca.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 01:09:23 2026 GMT
  host: api.drop.privacy.ca.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: California Privacy Protection Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for California Privacy Protection Agency, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: California Privacy Protection Agency
provider_slug: california-privacy-protection-agency
slug: california-privacy-protection-agency-domain-security
source_filename: california-privacy-protection-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cppa.ca.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: privacy.ca.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 03:16:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.drop.privacy.ca.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 01:09:23 2026 GMT\n  hsts: null\ndomains:\n- domain: ca.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/california-privacy-protection-agency/refs/heads/main/security/california-privacy-protection-agency-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Government
- Privacy
- Data Brokers
- Regulatory Compliance
- Data Deletion
- Consumer Rights
- California
- Webhook
---
