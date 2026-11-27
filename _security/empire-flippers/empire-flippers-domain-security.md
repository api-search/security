---
api_specs:
- filename: empire-flippers-openapi-generated.yml
  format: yaml
  label: Empire Flippers API
  slug: empire-flippers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empire-flippers/openapi/_ae-authored/empire-flippers-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: empireflippers.com
  spf: true
hosts:
- cert_expires: Jan  2 19:08:32 2027 GMT
  host: empireflippers.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Empire Flippers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Empire Flippers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Empire Flippers
provider_slug: empire-flippers
slug: empire-flippers-domain-security
source_filename: empire-flippers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: empireflippers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 19:08:32 2027 GMT\n  hsts: false\ndomains:\n- domain: empireflippers.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/empire-flippers/security/empire-flippers-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Marketplace
- Mergers and Acquisitions
- Online Business
- Software-as-a-Service
---
