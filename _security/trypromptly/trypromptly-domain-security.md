---
api_specs:
- filename: trypromptly-openapi-generated.yml
  format: yaml
  label: TryPromptly API
  slug: trypromptly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trypromptly/openapi/_ae-authored/trypromptly-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trypromptly.com
  spf: true
hosts:
- host: trypromptly.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''trypromptly'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trypromptly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TryPromptly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TryPromptly
provider_slug: trypromptly
slug: trypromptly-domain-security
source_filename: trypromptly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trypromptly.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''trypromptly'\n  hsts: null\ndomains:\n- domain: trypromptly.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/trypromptly/security/trypromptly-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Artificial Intelligence
- Prompt Engineering
- Software-as-a-Service
- Developer Tools
- Marketing
---
