---
api_specs:
- filename: identifai-net-openapi-generated.yml
  format: yaml
  label: identifAI API
  slug: identifai-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identifai-net/openapi/_ae-authored/identifai-net-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: identifai.net
  spf: true
hosts:
- cert_expires: Dec 23 14:42:26 2026 GMT
  host: identifai.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: identifAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for identifAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: identifAI
provider_slug: identifai-net
slug: identifai-net-domain-security
source_filename: identifai-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: identifai.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 14:42:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: identifai.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/identifai-net/security/identifai-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Deepfake Detection
- Enterprise
- Security
---
