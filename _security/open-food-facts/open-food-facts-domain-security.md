---
api_specs:
- filename: open-food-facts-openapi.yml
  format: yaml
  label: Open Food Facts
  slug: open-food-facts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openfoodfacts.org
  spf: true
hosts:
- cert_expires: Sep 19 15:07:01 2026 GMT
  host: world.openfoodfacts.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Food Facts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Food Facts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open Food Facts
provider_slug: open-food-facts
slug: open-food-facts-domain-security
source_filename: open-food-facts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: world.openfoodfacts.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:07:01 2026 GMT\n  hsts: false\ndomains:\n- domain: openfoodfacts.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/security/open-food-facts-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
