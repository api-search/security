---
api_specs:
- filename: dns-coffee-auth-api-openapi.yml
  format: yaml
  label: DNS Coffee Auth API
  slug: dns-coffee-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-auth-api-openapi.yml
- filename: dns-coffee-dnssec-api-openapi.yml
  format: yaml
  label: DNS Coffee Dnssec API
  slug: dns-coffee-dnssec-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-dnssec-api-openapi.yml
- filename: dns-coffee-domains-api-openapi.yml
  format: yaml
  label: DNS Coffee Domains API
  slug: dns-coffee-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-domains-api-openapi.yml
- filename: dns-coffee-feeds-api-openapi.yml
  format: yaml
  label: DNS Coffee Feeds API
  slug: dns-coffee-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-feeds-api-openapi.yml
- filename: dns-coffee-ips-api-openapi.yml
  format: yaml
  label: DNS Coffee Ips API
  slug: dns-coffee-ips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-ips-api-openapi.yml
- filename: dns-coffee-nameservers-api-openapi.yml
  format: yaml
  label: DNS Coffee Nameservers API
  slug: dns-coffee-nameservers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-nameservers-api-openapi.yml
- filename: dns-coffee-records-api-openapi.yml
  format: yaml
  label: DNS Coffee Records API
  slug: dns-coffee-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-records-api-openapi.yml
- filename: dns-coffee-search-api-openapi.yml
  format: yaml
  label: DNS Coffee Search API
  slug: dns-coffee-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-search-api-openapi.yml
- filename: dns-coffee-stats-api-openapi.yml
  format: yaml
  label: DNS Coffee Stats API
  slug: dns-coffee-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-stats-api-openapi.yml
- filename: dns-coffee-trends-api-openapi.yml
  format: yaml
  label: DNS Coffee Trends API
  slug: dns-coffee-trends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-trends-api-openapi.yml
- filename: dns-coffee-zones-api-openapi.yml
  format: yaml
  label: DNS Coffee Zones API
  slug: dns-coffee-zones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-zones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dns.coffee
  spf: false
hosts:
- cert_expires: Sep  5 05:38:03 2026 GMT
  host: dns.coffee
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 05:38:03 2026 GMT
  host: api.dns.coffee
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: DNS Coffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNS Coffee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: DNS Coffee
provider_slug: dns-coffee
slug: dns-coffee-domain-security
source_filename: dns-coffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dns.coffee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:38:03 2026 GMT\n  hsts: false\n- host: api.dns.coffee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:38:03 2026 GMT\n  hsts: false\ndomains:\n- domain: dns.coffee\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dns-coffee/security/dns-coffee-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DNS
- Domain Names
- Domains
- Zone Files
- Nameservers
- Research
---
