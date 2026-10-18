---
api_specs:
- filename: chronogg-attributions-api-openapi.yml
  format: yaml
  label: Chronogg Attributions API
  slug: chronogg-attributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-attributions-api-openapi.yml
- filename: chronogg-bounties-api-openapi.yml
  format: yaml
  label: Chronogg Bounties API
  slug: chronogg-bounties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-bounties-api-openapi.yml
- filename: chronogg-chronogg-api-api-openapi.yml
  format: yaml
  label: Chronogg Chronogg API
  slug: chronogg-chronogg-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-chronogg-api-api-openapi.yml
- filename: chronogg-code-api-openapi.yml
  format: yaml
  label: Chronogg Code API
  slug: chronogg-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-code-api-openapi.yml
- filename: chronogg-complete-reward-api-openapi.yml
  format: yaml
  label: Chronogg Complete Reward API
  slug: chronogg-complete-reward-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-complete-reward-api-openapi.yml
- filename: chronogg-event-api-openapi.yml
  format: yaml
  label: Chronogg Event API
  slug: chronogg-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-event-api-openapi.yml
- filename: chronogg-manage-api-openapi.yml
  format: yaml
  label: Chronogg Manage API
  slug: chronogg-manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-manage-api-openapi.yml
- filename: chronogg-member-api-openapi.yml
  format: yaml
  label: Chronogg Member API
  slug: chronogg-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-member-api-openapi.yml
- filename: chronogg-player-api-openapi.yml
  format: yaml
  label: Chronogg Player API
  slug: chronogg-player-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-player-api-openapi.yml
- filename: chronogg-rewards-api-openapi.yml
  format: yaml
  label: Chronogg Rewards API
  slug: chronogg-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/openapi/chronogg-rewards-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nexus.gg
  spf: true
hosts:
- cert_expires: Dec 10 18:43:26 2026 GMT
  host: www.nexus.gg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chronogg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chronogg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chronogg
provider_slug: chronogg
slug: chronogg-domain-security
source_filename: chronogg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexus.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 18:43:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nexus.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chronogg/refs/heads/main/security/chronogg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
