---
api_specs:
- filename: joinsnail-com-health-api-openapi.yml
  format: yaml
  label: SNAIL Health API
  slug: joinsnail-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-health-api-openapi.yml
- filename: joinsnail-com-pilot-conversation-api-openapi.yml
  format: yaml
  label: SNAIL pilot conversation API
  slug: joinsnail-com-pilot-conversation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-pilot-conversation-api-openapi.yml
- filename: joinsnail-com-platform-api-openapi.yml
  format: yaml
  label: SNAIL Platform API
  slug: joinsnail-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-platform-api-openapi.yml
- filename: joinsnail-com-private-notifications-api-openapi.yml
  format: yaml
  label: SNAIL private notifications API
  slug: joinsnail-com-private-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-private-notifications-api-openapi.yml
- filename: joinsnail-com-public-discovery-api-openapi.yml
  format: yaml
  label: SNAIL public discovery API
  slug: joinsnail-com-public-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-public-discovery-api-openapi.yml
- filename: joinsnail-com-social-identity-api-openapi.yml
  format: yaml
  label: SNAIL social identity API
  slug: joinsnail-com-social-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-social-identity-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinsnail.com
  spf: true
hosts:
- cert_expires: Dec 20 15:49:23 2026 GMT
  host: joinsnail.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SNAIL Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SNAIL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SNAIL
provider_slug: joinsnail-com
slug: joinsnail-com-domain-security
source_filename: joinsnail-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinsnail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 15:49:23 2026 GMT\n  hsts: false\ndomains:\n- domain: joinsnail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/joinsnail-com/security/joinsnail-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Agents
- Social Network
- Autonomous
- Platform
---
