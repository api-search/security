---
api_specs:
- filename: bountyhunte-rs-openapi-generated.yml
  format: yaml
  label: BountyHunte.rs API
  slug: bountyhunte-rs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bountyhunte-rs/openapi/_ae-authored/bountyhunte-rs-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bountyhunte.rs
  spf: true
hosts:
- cert_expires: Jan 29 20:06:13 2027 GMT
  host: bountyhunte.rs
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bountyhunte Rs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BountyHunte.rs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BountyHunte.rs
provider_slug: bountyhunte-rs
slug: bountyhunte-rs-domain-security
source_filename: bountyhunte-rs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bountyhunte.rs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 20:06:13 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bountyhunte.rs\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bountyhunte-rs/security/bountyhunte-rs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Bug Bounty
- Security
- Auditing
- Blockchain
---
