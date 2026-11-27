---
api_specs:
- filename: brainfile-io-openapi-generated.yml
  format: yaml
  label: Brainfile API
  slug: brainfile-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brainfile-io/openapi/_ae-authored/brainfile-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brainfile.io
  spf: true
hosts:
- cert_expires: Dec 22 02:17:56 2026 GMT
  host: brainfile.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainfile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brainfile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brainfile
provider_slug: brainfile-io
slug: brainfile-io-domain-security
source_filename: brainfile-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brainfile.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 02:17:56 2026 GMT\n  hsts: false\ndomains:\n- domain: brainfile.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/brainfile-io/security/brainfile-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Automation
- Developer Tools
- Claude
- Productivity
---
