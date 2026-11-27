---
api_specs:
- filename: ipjudge-org-openapi-generated.yml
  format: yaml
  label: IP Judge API
  slug: ipjudge-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipjudge-org/openapi/_ae-authored/ipjudge-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ipjudge.org
  spf: true
hosts:
- cert_expires: Dec 28 15:47:09 2026 GMT
  host: ipjudge.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IP Judge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IP Judge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IP Judge
provider_slug: ipjudge-org
slug: ipjudge-org-domain-security
source_filename: ipjudge-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipjudge.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 15:47:09 2026 GMT\n  hsts: false\ndomains:\n- domain: ipjudge.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ipjudge-org/security/ipjudge-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IP
- Check
- Artificial Intelligence
- Privacy
---
