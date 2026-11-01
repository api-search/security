---
api_specs:
- filename: dryrun-security-openapi.yml
  format: yaml
  label: DryRun Simple API
  slug: dryrun-simple-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dryrun-security/openapi/dryrun-security-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaqprivatemarket.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dryrun.security
  spf: true
hosts:
- cert_expires: Dec 21 07:53:45 2026 GMT
  host: www.nasdaqprivatemarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 01:48:18 2027 GMT
  host: docs.dryrun.security
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: simple-api.dryrun.security
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dryrun Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DryRun Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DryRun Security
provider_slug: dryrun-security
slug: dryrun-security-domain-security
source_filename: dryrun-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaqprivatemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dryrun.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 01:48:18 2027 GMT\n  hsts: false\n- host: simple-api.dryrun.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nasdaqprivatemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dryrun.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dryrun-security/security/dryrun-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- DevOps
- PenetrationTesting
- VulnerabilityScanning
- Compliance
---
