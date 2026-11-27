---
api_specs:
- filename: google-cloud-dns-changes-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Changes API
  slug: google-cloud-dns-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-changes-api-openapi.yml
- filename: google-cloud-dns-policies-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Policies API
  slug: google-cloud-dns-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-policies-api-openapi.yml
- filename: google-cloud-dns-locations-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Cloud Dns Locations API
  slug: google-cloud-dns-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-locations-api-openapi.yml
- filename: google-cloud-dns-operations-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Cloud Dns Operations API
  slug: google-cloud-dns-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-operations-api-openapi.yml
- filename: google-cloud-dns-projects-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Cloud Dns Projects API
  slug: google-cloud-dns-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-projects-api-openapi.yml
- filename: google-cloud-dns-dnskeys-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Dns Keys API
  slug: google-cloud-dns-dnskeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-dnskeys-api-openapi.yml
- filename: google-cloud-dns-managedzoneoperations-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Managed Zone Operations API
  slug: google-cloud-dns-managedzoneoperations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-managedzoneoperations-api-openapi.yml
- filename: google-cloud-dns-managedzones-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Managed Zones API
  slug: google-cloud-dns-managedzones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-managedzones-api-openapi.yml
- filename: google-cloud-dns-outboundendpoints-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Outbound Endpoints API
  slug: google-cloud-dns-outboundendpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-outboundendpoints-api-openapi.yml
- filename: google-cloud-dns-responsepolicies-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Response Policies API
  slug: google-cloud-dns-responsepolicies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-responsepolicies-api-openapi.yml
- filename: google-cloud-dns-responsepolicyrules-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Response Policy Rules API
  slug: google-cloud-dns-responsepolicyrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-responsepolicyrules-api-openapi.yml
- filename: google-cloud-dns-resource-record-sets-api-openapi.yml
  format: yaml
  label: Google Cloud DNS Resource Record Sets API
  slug: google-cloud-dns-resource-record-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dns/openapi/google-cloud-dns-resource-record-sets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: dns.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Cloud DNS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud DNS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud DNS
provider_slug: google-cloud-dns
slug: google-cloud-dns-domain-security
source_filename: google-cloud-dns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dns.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-dns/security/google-cloud-dns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DNS
- Domain Names
- Google Cloud
- Name Resolution
- Networking
---
