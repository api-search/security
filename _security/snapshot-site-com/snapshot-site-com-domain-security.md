---
api_specs:
- filename: snapshot-site-com-openapi-generated.yml
  format: yaml
  label: snapshot-site-com API
  slug: snapshot-site-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapshot-site-com/openapi/_ae-authored/snapshot-site-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: snapshot-site.com
  spf: true
hosts:
- cert_expires: Dec 28 02:02:36 2026 GMT
  host: snapshot-site.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Snapshot Site Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for snapshot-site-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: snapshot-site-com
provider_slug: snapshot-site-com
slug: snapshot-site-com-domain-security
source_filename: snapshot-site-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapshot-site.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 02:02:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: snapshot-site.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/snapshot-site-com/security/snapshot-site-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Screenshot
- API
- AI
- Monitoring
---
